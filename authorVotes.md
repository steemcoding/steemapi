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
  var dt = new Date();  //현재시간
  var end = dt.toISOString().split('.')[0];
  dt.setDate(dt.getDate() - 1); //하루전시간
  var start = dt.toISOString().split('.')[0];
 
  for(d in accountVotes){
    if(accountVotes[d].time>=start && accountVotes[d].time<=end){
      var data = accountVotes[d].authorperm.split('/');
      var author = data[0];
      var permlink = data[1];
      console.log(author+'/'+permlink+'/'+accountVotes[d].time);
      cnt+=1;
   }
  }
  console.log("count : " + cnt);
  
});
```
-----
## 결과
-----
```
minyool/18-04-30-ver/2018-04-30T22:48:15
bigman70/xdpwn/2018-05-01T04:16:42
carrotcake/editorial-illustration-for-creativecrypto-s-decentraland/2018-05-01T04:25:06
sjchoi/2018-5-1/2018-04-30T23:56:27
chosungyun/5dtahp/2018-05-01T12:04:24
armdown/1980/2018-05-01T05:56:09
codingman/5hqum8/2018-05-01T04:05:21
pyth0n/3ub9jw/2018-05-01T06:00:45
codingart/26-led/2018-05-01T12:13:06
hyyneeee/2ee97d/2018-05-01T12:40:15
kim0jh0/6wx9ur/2018-05-01T13:52:00
count : 11```
-----
