
## getRewardFund() 동작 ([BACK](README.md))
##### : 보상기금 정보보기로 name을 post로 검색하면 보상풀에 기금을 볼 수 있다.
-----
```
steem.api.getRewardFund(name, function(err, result) {
  console.log(err, result);
});
});
```
-----
## 명령
-----
```
steem.api.getRewardFund('post', function(err, result) {
  console.log(err, result);
});
 
```
## 결과
-----
```
null
[object Object] {
  author_reward_curve: "linear",
  content_constant: "2000000000000",
  curation_reward_curve: "square_root",
  id: 0,
  last_update: "2018-04-22T09:51:54",
  name: "post",
  percent_content_rewards: 10000,
  percent_curation_rewards: 2500,
  recent_claims: "439748733835456845",
  reward_balance: "749384.376 STEEM"
}
```
-----
