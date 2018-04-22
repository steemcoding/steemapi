
## getFeedHistory() 동작 ([BACK](README.md))
##### : 평균 base와 quote의 price 정보를 가져온다.
-----
```
steem.api.getFeedHistory(function(err, result) {
  console.log(err, result);
});
```
-----
## 명령
-----
```
steem.api.getFeedHistory(function(err, result) {
  console.log(err, result);
});
 
```
## 결과
-----
```
null
[object Object] {
  current_median_history: [object Object] {
    base: "3.012 SBD",
    quote: "1.000 STEEM"
  },
  id: 0,
  price_history: [[object Object] {
  base: "2.900 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.892 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.905 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.020 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.029 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.049 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.050 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.012 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.957 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.933 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.919 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.891 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.893 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.945 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.946 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.023 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.962 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.953 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.973 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.983 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.992 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.992 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.012 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.966 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.003 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.003 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.990 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.019 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.962 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.951 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.951 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.976 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.010 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.053 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.053 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.068 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.069 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.025 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.017 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.022 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.038 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.065 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.056 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.140 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.101 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.148 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.084 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.090 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.107 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.107 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.065 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.063 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.060 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.082 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.012 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.952 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.878 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.885 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.900 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.929 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.006 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.016 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.991 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.995 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.998 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.015 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.934 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.015 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.020 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.015 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.969 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.990 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.955 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.953 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.901 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.973 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "2.973 SBD",
  quote: "1.000 STEEM"
}, [object Object] {
  base: "3.020 SBD",
  quote: "1.000 STEEM"
}]
}
```
-----
