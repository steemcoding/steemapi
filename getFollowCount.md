## getFollowCount() 동작 ([BACK](README.md))
##### : 팔로우 정보를 가져옴.
-----
```
steem.api.getFollowCount(author, function(err, result) {
     console.log(result);
});
```
-----
## 명령
-----
```
var author = 'codingman';
steem.api.getFollowCount(author, function(err, result) {
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
