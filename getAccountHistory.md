
## getAccountHistory() 동작 ([BACK](README.md))
##### : account(id)에게 가장 최근에 행동을 보여 준 스티미언 정보를 limit(횟수)만큼 보여준다.
-----
```
steem.api.getAccountHistory(account, from, limit, function(err, result) {
  console.log(err, result);
});
```
-----
## 명령
-----
```
var account ='codingman';
var from = -1;
var limit = 3;
steem.api.getAccountHistory(account, from, limit, function(err, result) {
  console.log(err, result);
});

 
```
## 결과
-----
```
null
[[8913, [object Object] {
  block: 21784572,
  op: ["comment", [object Object] {
  author: "sh931216",
  body: "아두이노에 관심이 있어서 팔로우 하고 갈게요",
  json_metadata: "{\"tags\":[\"kr-arduino\"],\"app\":\"steemit/0.1\"}",
  parent_author: "codingman",
  parent_permlink: "switch-case",
  permlink: "re-codingman-switch-case-20180422t075419987z",
  title: ""
}],
  op_in_trx: 0,
  timestamp: "2018-04-22T07:54:21",
  trx_id: "9839b60c63738bd0fa0340ce4010de89efcf660a",
  trx_in_block: 7,
  virtual_op: 0
}], [8914, [object Object] {
  block: 21786713,
  op: ["vote", [object Object] {
  author: "codingman",
  permlink: "steem-js",
  voter: "soyo",
  weight: 500
}],
  op_in_trx: 0,
  timestamp: "2018-04-22T09:41:27",
  trx_id: "43d14af343c76499af58534534fb283c4284b6e0",
  trx_in_block: 18,
  virtual_op: 0
}], [8915, [object Object] {
  block: 21787261,
  op: ["curation_reward", [object Object] {
  comment_author: "jongeun",
  comment_permlink: "3ujjzm",
  curator: "codingman",
  reward: "4.074864 VESTS"
}],
  op_in_trx: 0,
  timestamp: "2018-04-22T10:08:54",
  trx_id: "0000000000000000000000000000000000000000",
  trx_in_block: 41,
  virtual_op: 0
}]]
```
-----

