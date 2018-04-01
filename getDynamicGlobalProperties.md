
## getDynamicGlobalProperties() 동작 ([BACK](README.md))
-----
```
steem.api.getDynamicGlobalProperties(function(err, result) {
  console.log(err, result);
});
```
-----

## 결과
-----
```
null { head_block_number: 21180421,
  head_block_id: '0143300507467810590a68039c7300f1fed5eca8',
  time: '2018-04-01T08:22:27',
  current_witness: 'netuoso',
  total_pow: 514415,
  num_pow_witnesses: 172,
  virtual_supply: '273616455.312 STEEM',
  current_supply: '266268887.938 STEEM',
  confidential_supply: '0.000 STEEM',
  current_sbd_supply: '11249125.650 SBD',
  confidential_sbd_supply: '0.000 SBD',
  total_vesting_fund_steem: '189482041.869 STEEM',
  total_vesting_shares: '386481418928.609509 VESTS',
  total_reward_fund_steem: '0.000 STEEM',
  total_reward_shares2: '0',
  pending_rewarded_vesting_shares: '381709236.452311 VESTS',
  pending_rewarded_vesting_steem: '185970.596 STEEM',
  sbd_interest_rate: 0,
  sbd_print_rate: 7733,
  maximum_block_size: 65536,
  current_aslot: 21245249,
  recent_slots_filled: '340282366920938463463374607431768211455',
  participation_count: 128,
  last_irreversible_block_num: 21180405,
  vote_power_reserve_rate: 10,
  average_block_size: 11788,
  current_reserve_ratio: 200000000,
  max_virtual_bandwidth: '264241152000000000000' }
  ```
  -----
