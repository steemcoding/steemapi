
## 스티미언 블로그 전체 게시물 보기 ([BACK](README.md))
##### : steem.api.getDiscussionsByBlog() 함수을 이용하여 id(스티미언)의 블로그 게시물을 전체를 재귀함수로 가져온다.
-----
```
var query = {
  "tag": "codingman",
  "limit": 10
};
 steem.api.getDiscussionsByBlog(query, function(err, discussionsByBlog) {
  console.log(err, discussionsByBlog);
});
```
```
{ "tag": "codingman",
  "limit": 10,
  "start_author": "author",
  "start_permlink": "permlink" }
```
-----
## 명령
-----
```

var query = {
  "tag": "codingman",
  "limit": 10
};

var cnt=0;

(function run(){
  steem.api.getDiscussionsByBlog(query, function(err, discussionsByBlog) {    

    for(var i=0;i<discussionsByBlog.length-1;i++){
      console.log(err, discussionsByBlog[i].title);     
    }

    cnt=discussionsByBlog.length;

    if(cnt<10){
      console.log(err, discussionsByBlog[cnt-1].title);     
      return;
    }
    else{
      query.start_author= discussionsByBlog[cnt-1].author;
      query.start_permlink= discussionsByBlog[cnt-1].permlink;
      //console.log(query);

      run();
    }
  });
})();


```
## 결과
-----
```
null '조이스틱+processing 3D 도형 회전(아두이노)'
null '조이스틱 방향키 값 출력(아두이노)'

.....

null 'STEEMIT 첫인사'

```
-----
