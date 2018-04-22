## getFollowers() 동작 ([BACK](README.md))
##### : 팔로우 정보를 가져옴.
-----
```
steem.api.getFollowers(following, startFollower, followType, limit, function(err, result) {
  console.log(err, result);
});
```
-----
## 명령
-----
```
var following = 'codingman';
var startFollower = 0;
var followType = 'blog';
var limit = 3;
steem.api.getFollowers(following, startFollower, followType, limit, function(err, result) {
	console.log(result);
});
```
## 결과
-----
```
[[object Object] {
  follower: "a-0-0",
  following: "codingman",
  what: ["blog"]
}, [object Object] {
  follower: "a-0-0-0-1abokina",
  following: "codingman",
  what: ["blog"]
}, [object Object] {
  follower: "a-0-0-0-a",
  following: "codingman",
  what: ["blog"]
}]
```
-----
