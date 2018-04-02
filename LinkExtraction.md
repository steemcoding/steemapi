## 전체 링크주소에서 author, Permlink 추출([BACK](README.md))

 ##### : author(저자), Permlink(게시물주소이름)을 주로 사용하는데 link된 전체주소에서 author와 Permlink를 추출할 수 있다.
-----
```
var author = 'id';
var permlink = 'postlink name';
```

-----
## 명령
-----
```
 var link = 'https://steemit.com/kr/@codingman/steemit'
 var arrlink = link.split('/');
 var idlink = arrlink[arrlink.length-2].replace('@','');

 var author = idlink;
 var permlink =  arrlink[arrlink.length-1];
	
console.log('author : ' + author);
console.log('permlink : ' + permlink);
 
```
-----
## 결과
-----
```
author : codingman
permlink : steemit
```
-----
