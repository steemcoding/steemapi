## getFollowCount() 동작 ([BACK](README.md))
##### : 팔로우와 팔로워 숫자 추출함.
-----
```
steem.api.getFollowCount(account, function(err, result) {
     console.log(result);
});
```
-----
## 명령
-----
```
var account = 'codingman';
steem.api.getFollowCount(account, function(err, result) {
     console.log(result);
});
```
## 결과
-----
```
[object Object] {
  account: "codingman",
  follower_count: 671,
  following_count: 438
}
```
-----
