
## lookupAccounts() 동작 ([BACK](README.md))
##### : lowerBundName(아디철자)를 기준으로 가까운 이름들 출력한다. limit(출력수)
-----
```
steem.api.lookupAccounts(lowerBoundName, limit, function(err, result) {
  console.log(err, result);
});
```
-----
## 명령
-----
```
steem.api.lookupAccounts('coding', 20, function(err, result) {
  console.log(err, result);
});
```
## 결과
-----
```
null [ 'coding',
  'coding-lion',
  'coding-school',
  'codingauthority',
  'codingbob',
  'codingcode',
  'codingconvention',
  'codingdaddy',
  'codingdefined',
  'codingdoctor',
  'codingdodo',
  'codinggeeks',
  'codingguy',
  'codingholic',
  'codinghusi',
  'codinginmysleep',
  'codingman',
  'codingmarco',
  'codingmonster',
  'codingnick' ]

```
-----
