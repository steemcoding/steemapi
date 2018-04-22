## SP 구하기 ([BACK](README.md))
##### : steem.api.getAccounts(), steem.api.getDynamicGlobalProperties()함수로 해당 스티미언의 SP를 계산한다.
-----
### 스티미언 정보 - vesting_shares
```
var author = 'codingman';
steem.api.getAccounts([author], function (err, accounts) {
	console.log(accounts);
});
```
###  Global 속성정보 - total_vesting_fund_steem, total_vesting_shares
```
steem.api.getDynamicGlobalProperties(function (err, globalProperties) {
	console.log(globalProperties);
});
```
-----
## SP 계산식

```
 SP = total_vesting_fund_steem/total_vesting_shares*vesting_shares;
```
-----
## 명령
-----
```
steem.api.getAccounts(['codingman'], function (err, accounts) {
  var vesting_shares = parseFloat(accounts[0].vesting_shares.split(" ")[0]);
  
  steem.api.getDynamicGlobalProperties(function (err, globalProperties) {
    var total_vesting_fund_steem = parseFloat(globalProperties.total_vesting_fund_steem.split(" ")[0]);
    var total_vesting_shares = parseFloat(globalProperties.total_vesting_shares.split(" ")[0]);

    var SP =((total_vesting_fund_steem/total_vesting_shares)*vesting_shares).toFixed(2);
    console.log(SP);
  });  
});


```
## 결과
-----
```
272.24

```
-----
