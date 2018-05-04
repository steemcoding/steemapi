## 현재시간으로 부터 24시간동안 보팅한 내역 조사 ([BACK](README.md))

 ##### : author(저자), Permlink(게시물주소이름), time(보팅시간)의 정보를 함께 얻을 수 있다.
-----
```
var author = 'codingman';
steem.api.getAccountVotes(author, function(err, accountVotes) {
	console.log(err, accountVotes);
}
```

-----
## 명령
-----
```
var author = 'codingman';

steem.api.getAccountVotes(author, function(err, accountVotes) {
   // console.log(err, accountVotes);

  var cnt = 0;
  var dt = new Date();  
  var endTime = dt.toISOString().split('.')[0];

  dt.setDate(dt.getDate() - 1);
  var startTime = dt.toISOString().split('.')[0];


  console.log(startTime+' ~ '+endTime+'\n');

  for(d in accountVotes){
    if(accountVotes[d].time>=startTime && accountVotes[d].time<=endTime){
      var data = accountVotes[d].authorperm.split('/');
      var author = data[0];
      var permlink = data[1];

      console.log('['+author+'] '+permlink+' ('+accountVotes[d].time+')');
      cnt+=1;

   }
  }
  console.log("\n count : " + cnt);

});
```
-----
## 결과
-----
```
2018-05-03T15:21:19 ~ 2018-05-04T15:21:19

[jisung] 2jd4xu-1 (2018-05-04T07:11:18)
[saloon1st] 4fxrzm (2018-05-04T07:13:18)
[carrotcake] k33kn (2018-05-04T08:20:30)
[urobotics] 1-unity (2018-05-04T07:17:48)
[kookmin] -27458183e6f16 (2018-05-04T04:18:24)
[virus707] 71ehmr-5-3 (2018-05-04T04:11:51)
[song1] 55dj92 (2018-05-04T04:22:18)
[sjchoi] 2018-5-4 (2018-05-04T04:15:12)
[codingman] 6hy1ml-processing-3d (2018-05-04T04:06:06)
[segyepark] bwo5e (2018-05-04T12:05:18)
[kim0jh0] 6f5m9d (2018-05-04T14:18:39)

count : 11
```
-----
