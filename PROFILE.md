## PROFILE 정보 읽기 ([BACK](README.md))

 ##### : steem.api.getAccounts()함수에서 해당 스티미언의 프로파일 정보를 가져온다. 참고로 JSON형태로 변환 시키면 접근자로 쉽게 해당 데이터를 접근할 수 있다.
-----
```
steem.api.getAccounts(['id'], function(err, response){
    var obj = JSON.parse(response[0].json_metadata);
    console.log(err, obj.profile);
});

```
-----
## 명령
-----
```
steem.api.lookupAccountNames(['codingman'], function(err, result) {
  console.log(err, result);
});
```
-----
## 결과
-----
```
null { name: '천간',
  about: '나는 소망한다 내게 주어진 모든것들을',
  profile_image: 'https://i.imgsafe.org/85/850796af2e.png',
  cover_image: 'https://i.imgsafe.org/85/8504d5e392.jpeg' }
```
-----
