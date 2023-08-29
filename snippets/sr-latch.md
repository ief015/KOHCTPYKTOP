# S/R Latches

## Accurate

A large, but accurate SR latch. Rising/falling lag of 0/1.

```
eNrtWltywyAMrFn/5Ay9Qv9zlt7/Ik3dZGrHeMFSeGTYOP7w7AiExC6yYf6aPy/f
0+U6zR+Wa0zDYDec7tdpw//rlGFGb+PmcRTDYDdMztcjw+R8jRua2NEmqmZXzcFx
pEPsGNbQvASYFx3HMqc8ug2Xci4c/xYUQPT2ozf88Q/3p1W/Gejtpuhfb1h63KIL
FB8vj8aoKDgKsJbBbH9nosNr2P2CMpyBcq4keJbiqJH9JTXpKBpZYtkxCk3pSig0
IqEjM/TdpTJNB1J1QFP6dehzpCvVb3B4pQzmonCwTFLZyaoEShbs8XXLqitOVFkk
krFI16FSomXqFR+R5kY2UyjLOEMhqawllVDdWEkq0apudFSV3GeJ4WuqSs5BvYD3
s96xNQu77/obVHQ4Vb+xGmwX6S1azCsuldyrwDejlP08piRYVjD7/Ull213u1B54
YLaqHOp9FWzjMxw+C83ZAac8yuBgZzvghaUyfvvRGi+V21MMqyMQokM1yZJXb31Y
yMyyUl41UKQfcL7Haw==
```

![06 KL2S1 DUAL SET-RESET LATCH - variants](./assets/sr-latch-accurate.png)

## Compact

A compact SR latch in two flavours.

- Output from latch core via (left, bottom snippets)
  - Rising/falling lag: 1/1
  - Output via somewhat awkward to reach.
- Output from bottom metal (right, top snippets)
  - Rising/falling lag: 1/2
  - Output easier to access at the expense of extra lag.

```
eNrtWkt2gzAMrDVscoZeIfuepfe/SNtA3iuJJMeWATuMCRsm/kmasXhiuk6fl+90
+UrTR8111o5S1zEtV9WMkp9V32OiH8/dMeWDIRdyZvj5Qe4EfI5WMo4CSJ0CFBun
yh2BACCt3lEBtj90Qscc/RjseEvnxG43FIB6x9FfXOb/zA2ree+oWOg8mIGKO7K4
Iy/P/kzkjX1vCmrZcmQUa1sUoVzz4Ch8FAa6cNRgSobfDoO31CTLGi+JJVGiRIme
Gx1eKhE5DRkApXkFPC+gy9hA1Y7o/VY5JyiVXYghFHzVFxTSJmK4vBDpr6v499tV
SN2RM6tyd0QhLWIKAgylVO6UNzKr7CFvPCqrDK2KYrhL3sissg8U8J1IqWwlSniy
56MXAHQYG+aq3B3R+8WxUcfQN5PKBlVuqaxyrx6qteZYlbsaPR9ZRqwXs8Z9cAXc
5e8LFXBpXwHfWCr1O47GXpO1A2u/k/TxCwgSjShRjaEBpuAgRXpuP6FVx1k=
```

![06 KL2S1 DUAL SET-RESET LATCH - variants](./assets/sr-latch-compact.png)

## Extra Compact

A very compact and accurate (Rising/falling lag: 0/1 or 0/2) SR latch. This SR latch causes the SET
pin to short circuit with VCC, causing SET to stay high until RESET.

Using the bottom pins allow easier access to the output, but introduces an increased falling lag
of 2. Connecting the output directly with the SET input results with a small falling lag of 1,
making this design one of the most accurate.

Because of the short circuit, it is not recommended to use this design unless aiming for a low
design score, or you are not worried about the circuit of the SET input.

```
eNrtmlEOgyAQRAvjj2foFfrfs/T+F2mDNo0Nu+iuSoSR+NOXDcgywxI6PIb7+Arj
Mww3S+s3MNgCY2qbA8PcmA4Gnh4YbIGFpS4FFpd6A7Pq+EbjrDrySHV0GujYdIzb
nGNjZR6/gamci/KTKIDs66cfnl7M3WHR70yhUjkWqS+BLn7L09+TodJcdUzhoL2N
qhk6yQMSnRQq6Miu7iMdSfreVVZJSkpK2je9vlVCo2CKT6PQKCqNCo4xM78rKRwK
pVWeaIaQqXI04ILf3QyVwywqHXUL/UIfFY10FS2oDLoGL2OkDVglF23XdSOrSlaV
tMpVadISAYBL+ixT0mwHqGNKhX5Bq9yjqtRVhp6s8vA77gKNptgYi3fcKqUcdr1r
5qiapMgXjjvo96gb8IOtMv/6qf8AriQxs51tq1f//+NAsZCSbleZqiOTuis40htY
IccB
```

![06 KL2S1 DUAL SET-RESET LATCH - variants](./assets/sr-latch-extra-compact.png)

## Simplified

A simplified SR latch for illustrative purposes. Rising/falling lag of 1/1.

```
eNrtWkESwiAMFNJL3+AXvPsW//8RbbAzIBAwhdrK2qk9bNJ0ssmSitNtus4PM9/N
dNEcJ3e0/G2+dTR8WD6+jmh1jiPQMYpjsezSjhVll49odY7gEY7aIleV3KYiV7UV
eOyxsKqWuU0Lq2op/0M6eJyz+Q+jRJQ8t6Mv3J3kwlEQl70Xc76yV4BKzzwqSl4S
P1BH+ZJOvuZMfNtUjBqLF7CWmM0YeTfIWYQBh4F9ltImQYJFMj0WMlY2MBKqLor0
64KXxWEVlvcj026KlnvoKqkFChQo0LHRE0hlNGeBxB4zK3IFFtDdR5dKMV1uRkej
tWjDOJfI5P5ogYWhhLTQ3UcS0uNL5fqjBRqtwcQS5RKZ7MUCxLCqfzFVNlx3eOHJ
p5oIr+fV80yUy7CFifBi2EYqpUwWWPg7qZQ6tNDdp5PKrnvkQTjskQMFOgoq976k
G332uJtIZfrcjhaTSS5Z4d8JUHhqFBM4WDiOVKq7+weK9ATIg8eV
```

![06 KL2S1 DUAL SET-RESET LATCH - variants](./assets/sr-latch-simplified.png)

## See Also

[06 KL2S1 DUAL SET-RESET LATCH](/levels/06%20KL2S1%20DUAL%20SET-RESET%20LATCH.md)