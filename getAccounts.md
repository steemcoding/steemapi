
## getAccounts() 동작 ([BACK](README.md))
##### : 여러명의 스티미언 정보를 가져 올 수 있다. 하지만, 한명의 스티미언 정보를 가져올 때도 사용한다
-----
```
steem.api.getAccounts(['name1','name2'], function(err, result){
    console.log(err, result);
});
```
-----
## 명령
-----
```
steem.api.getAccounts(['codingman'], function(err, result){
    console.log(err, result);
});
```
## 결과
-----
```
null [ { id: 496769,
    name: 'codingman',
    owner: { weight_threshold: 1, account_auths: [], key_auths: [Array] },
    active: { weight_threshold: 1, account_auths: [], key_auths: [Array] },
    posting: 
     { weight_threshold: 1,
       account_auths: [Array],
       key_auths: [Array] },
    memo_key: 'STM7nqrFBKwraxv8r69c5sVc9A39ZKwZUEL7cTGxdggXxokBWUJ8X',
    json_metadata: '{"profile":{"name":"천간","about":"나는 소망한다 내게 주어진 모든것들을","profile_image":"https://i.imgsafe.org/85/850796af2e.png","cover_image":"https://i.imgsafe.org/85/8504d5e392.jpeg"}}',
    proxy: '',
    last_owner_update: '1970-01-01T00:00:00',
    last_account_update: '2018-03-31T03:02:48',
    created: '2017-12-15T02:26:24',
    mined: false,
    recovery_account: 'steem',
    last_account_recovery: '1970-01-01T00:00:00',
    reset_account: 'null',
    comment_count: 0,
    lifetime_vote_count: 0,
    post_count: 1548,
    can_vote: true,
    voting_power: 7992,
    last_vote_time: '2018-04-01T07:45:27',
    balance: '0.317 STEEM',
    savings_balance: '0.000 STEEM',
    sbd_balance: '21.692 SBD',
    sbd_seconds: '13422770328',
    sbd_seconds_last_update: '2018-04-01T04:08:21',
    sbd_last_interest_payment: '2018-03-22T04:20:33',
    savings_sbd_balance: '0.000 SBD',
    savings_sbd_seconds: '0',
    savings_sbd_seconds_last_update: '1970-01-01T00:00:00',
    savings_sbd_last_interest_payment: '1970-01-01T00:00:00',
    savings_withdraw_requests: 0,
    reward_sbd_balance: '0.000 SBD',
    reward_steem_balance: '0.000 STEEM',
    reward_vesting_balance: '6.119065 VESTS',
    reward_vesting_steem: '0.003 STEEM',
    vesting_shares: '432872.465212 VESTS',
    delegated_vesting_shares: '0.000000 VESTS',
    received_vesting_shares: '0.000000 VESTS',
    vesting_withdraw_rate: '0.000000 VESTS',
    next_vesting_withdrawal: '1969-12-31T23:59:59',
    withdrawn: 0,
    to_withdraw: 0,
    withdraw_routes: 0,
    curation_rewards: 969,
    posting_rewards: 87902,
    proxied_vsf_votes: [ 0, 0, 0, 0 ],
    witnesses_voted_for: 0,
    last_post: '2018-04-01T07:45:21',
    last_root_post: '2018-04-01T04:05:15',
    average_bandwidth: '191029868073',
    lifetime_bandwidth: '1973313000000',
    last_bandwidth_update: '2018-04-01T07:45:27',
    average_market_bandwidth: 1300000000,
    lifetime_market_bandwidth: '210780000000',
    last_market_bandwidth_update: '2018-03-29T04:10:09',
    vesting_balance: '0.000 STEEM',
    reputation: '1131871127262',
    transfer_history: [],
    market_history: [],
    post_history: [],
    vote_history: [],
    other_history: [],
    witness_votes: [],
    tags_usage: [],
    guest_bloggers: [] } ]
```
-----
