## POST에 보팅한 사람들 보팅액 계산 ([BACK](README.md))
##### :  특정 post에 보팅한 사람들의 보팅 금액을 계산한다. 


-----
 - 출처 : https://cnsteem.com/kr/@tradingideas/node-js-3
-----

## 사용 함수
-----
### 보팅자 정보
```
steem.api.getActiveVotes(author, permlink, function (err, activeVoters) {
		console.log(err,activeVoters);
});
```
### 보상풀에 reward_balance, recent_claims 정보
```
steem.api.getRewardFund("post", function (err, rewardFund) {  
		console.log(err,rewardFund);
});
```
### historyPrice의 base, quote 기준 정보
```
steem.api.getCurrentMedianHistoryPrice(function (err, historyPrice) {
	 console.log(err,historyPrice);
});
```

보팅한 사람의 금액 계산식

##### : 기준이 되는 baseSBD 값을 구한 값에다 votoer의 보팅한 shares 값을 곱한 값
-----
baseSBD = (reward_balance/recent_claims) \* (base/quote) 

voterSBD = baseSBD \* (activeVoters[i].rshares)

-----

## 명령
-----
```
var author = 'codingman'
var permlink = 'steemit'
steem.api.getActiveVotes(author, permlink, function (err, activeVoters) {
    var voterSBD, baseSBD;
    var msg = "voters : " + activeVoters.length;    
    console.log(msg);
    
    steem.api.getRewardFund("post", function (err, rewardFund) { 
      var reward_balance = parseFloat(rewardFund.reward_balance.split(' ')) 
      var recent_claims = parseInt(rewardFund.recent_claims) 
      
      baseSBD = reward_balance/recent_claims;
      
      steem.api.getCurrentMedianHistoryPrice(function (err, historyPrice) {
        var basePrice = parseFloat(historyPrice.base.split(' ')) 
        var quotePrice = parseFloat(historyPrice.quote.split(' ')) 
        
        baseSBD = baseSBD*basePrice/quotePrice;
      
        // voters 계산
        for (var i = 0; i < activeVoters.length; i++) {   
          var rshares = parseInt(activeVoters[i].rshares) 
        
          voterSBD = (baseSBD * rshares).toFixed(2);  
         
          var output = activeVoters[i].voter + ' : ($' + voterSBD + ')';
          console.log(output);
        }
      });     
    });    
});
```
## 결과
-----
```
voters : 15
woo7739 : ($0.12)
abdullar : ($1.82)
saloon1st : ($0.01)
coolzero : ($0.04)
zinasura : ($1.03)
mastertri : ($0.15)
toppy : ($0.01)
mokko : ($0.00)
yibt5227 : ($0.01)
kaine : ($0.00)
bobkook : ($0.00)
myfan : ($0.00)
sirsubk1014 : ($0.01)
spiritboxer : ($0.01)
codingman : ($0.01)
```
-----
