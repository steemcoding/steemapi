## getActiveVotes() ([BACK](README.md))

 ##### : author(저자), Permlink(게시물주소이름)을 통해 해당 게시물의 업보팅한 스티미언 정보를 가져온다.
-----
```
var author = 'id';
var permlink = 'postlink name';

steem.api.getActiveVotes(author, permlink, function (err, result) {
		console.log(err, result);
});
```
-----
## 명령
-----
```
var author = 'codingman';
var permlink = 'steemit';

steem.api.getActiveVotes(author, permlink, function(err, result) {
		console.log(err, result);
});
```
-----
## 결과
-----
```
null [ { voter: 'Voter1',
    weight: 23215,
    rshares: '24342459101',
    percent: 100,
    reputation: '65419965993115',
    time: '2017-12-16T15:29:21' },
  { voter: 'Voter2',
    weight: 317191,
    rshares: '361170022544',
    percent: 1000,
    reputation: '165559015464652',
    time: '2017-12-16T15:30:48' },
  { voter: 'Voter3',
    weight: 1626,
    rshares: 2428541594,
    percent: 10000,
    reputation: '2694892101198',
    time: '2017-12-15T09:05:30' },
  { voter: 'Voter4',
    weight: 6762,
    rshares: '7091055653',
    percent: 3000,
    reputation: '12738878905785',
    time: '2017-12-15T13:15:12' },
  { voter: 'Voter5',
    weight: 372338,
    rshares: '204336686145',
    percent: 10000,
    reputation: '2747131642942',
    time: '2017-12-15T12:28:33' }
		.....
		                                     ]
```
-----
