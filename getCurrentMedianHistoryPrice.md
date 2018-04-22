
## getCurrentMedianHistoryPrice() 동작 ([BACK](README.md))
##### : 평균 base와 quote의 price 정보만 가져온다.
-----
```
steem.api.getCurrentMedianHistoryPrice(function(err, result) {
  console.log(err, result);
});
```
-----
## 명령
-----
```
steem.api.getCurrentMedianHistoryPrice(function(err, result) {
  console.log(err, result);
});
 
```
## 결과
-----
```

null
[object Object] {
  base: "3.012 SBD",
  quote: "1.000 STEEM"
}
```
-----
