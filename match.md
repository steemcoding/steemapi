## 게시물에서 특정 문자열 찾기 ([BACK](README.md))
##### : steem.api.getContent()함수로 해당 게시물에 특정 문자열을 찾는 방법
##### 불특정 실시간 게시물에서 찾기 위해서는 다른 함수를 사용해야 합니다.
-----
```
var str = result['body'];
if(str.match('특정문자열')) console.log("찾았다");
```
-----
## 명령
-----
```
steem.api.getContent('codingman', '5kszkb', function (err, result) {

	var str = result['body'];
	if(str.match('자료형')) console.log("찾았다");

});

```
## 결과
-----
```
"찾았다"

```
-----
