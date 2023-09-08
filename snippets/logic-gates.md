# Logic Gates

- [NOT Gate](#not-gate)
- [AND Gate](#and-gate)
- [NAND Gate](#nand-gate)
- [OR Gate](#or-gate)
- [NOR Gate](#nor-gate)
- [XOR Gate](#xor-gate)
- [XNOR Gate](#xnor-gate)

## NOT Gate

Output is high if input is low, and vice-versa.

```
eNrt2UEOgjAUBUDLZ8MZvAJ7z+L9L6I2LtvUUAhqB+hq8iDQ5AHpvM7X5Z6WW5ov
W/Yxg2lbcMq7pyooKCgoKCi4ezB/zk31LWtEFEe/Pj0f5es29XWuqr7zlNI/0yMb
qdaEH1UlpZSOrb9elWESKaWqslGGrR9wU0wpVZUmkVKqKtsaipRS+i1VeeIad/Om
rAlSOpoes8a9S1WWR7/29X+E9x2l4+kJjfQA0SLGgw==
```

![Logic NOT](./assets/logic-not.png)

## AND Gate

Output is high if all inputs are high, else output is low.

### 2-Input

The larger variant on the left provides a stable output, while the smaller variant on the right has
varying lag characteristics due to propegation delay, which can also create unintended spikes in
some cases.

```
eNrtmW8OgyAMxSf1i2fYFfZ9Z9n9LzIl/oHSAo4ZUZ7OZMnvFbQtTxL7V/8cPt3w
7vrHL2ergWa+dgZ264msIhCBCEQgAm8dGHndpWY0yOovgXY7Z/TDUiISr3I6cls4
sr/5H58+VzQeM7YTBAIj9IgoM5pCGcqoGjWlWVgUuHdZhiWB0w2iwO2WJA4FXrPF
UqcIWLMGAt7MQX3CbvcFwmrwBHJ8RJC4A6GBWAkiWVLwqtDoIlCpP0BGn2b0SmrN
aY+sZZyNuD4QPydTWKyBPXsg3Yxmu4ktE87UnhUx7ZFuqVUry8ZBQUFB26aXt8rp
LYUSg4LWTQlWebIZEq8C2hIUtDrqL+JLGunVrRJtCQqKXSWsMkn51yW0JShohbvK
Rqyy9Pv7sjOU0pWmd3krgYK2SslfwwGlnfSYb9x/sUr5KqdlhZh3lHxjiaYFBa3N
Kt1VWjzyCY70Bc87x7Q=
```

![Logic AND 2-input](./assets/logic-and-2.png)

### 4-Input

Add or remove NPN gates to desired number of inputs. This design illustrates a 4-input AND gate.

Although it is possible to use one of the inputs in place of VCC, it can cause varying lag
characteristics and produce unintended spikes similar to the 2-input single-NPN gate shown
above.

```
eNrtmUsWgyAMRYUwcQ3dQuddS/e/kXpSqT+irfipekEGenmK0fOMJ+EebuXTlQ8X
ijkdIcJlhb7uPwpdqxNVhAgRIkR4QaGmc95uSkUkOfJpxb3OET2me8113/uhiBNk
BA9XvQkOxRj3tlpbdfrWPbdwndLoAowZn3Y22otYn3p/Llq9Qf+KDxTONS3Kssav
vBMKhUKvTbHKXaiVfRIrKBSrxAw7/xRCrKBQrBKrJG+EQrFKaA4VjBQKPaFVLlD0
jluy6N2UQU06p+q8K51+EAJNMyh0gq5T417EKtMjn8Ykqz5mL7ubhx34mzVMKPmC
Tz59YgXd1JES7QUzx8cQ
```

![Logic AND 4-input](./assets/logic-and-4.png)

## NAND Gate

Output is low if all inputs are high, else output is high.

### PNP Design

By using multiple PNP gates (one for every input) with a shared output, we create a NAND gate
with a low rising/falling lag of 1/1.

```
eNrtmVGSgjAMhqU/L57BK+y7Z/H+F1laXCi1yZZCUcxfZJzxS9ImtSEZ+p/+dn10
13vXX2ouKn6sostcK2bsgkI3fa9YauWM3McTKL7saZli5l/UeEY727E4auu2I9qW
xjPyWFGRiocohnLOySNQANl7Ox348PErgR/jooaveHYvE370QpFoKuNikdlF3dTE
VZlYao5XiUz0OMJrYJdCiZGliIvckkRCXEUDqfnduWtr/uzcEX8aTo/TAflOyrNF
idgm9dFTMxtjlaFTxL7Ko+AV99c0ZaokJSUlZaqUKP7TfdYS0CybrDmh0Tliecs4
pUejV7Jl1pxMlZZbbDbgNS32GRtwvcVmA05qu6r8G3JVOV5iIlV0LVeVqNZ9Y6p8
7qXkERyqdJl2rKXK7W/Qx0OCzGHB1OI4lSLfRFfTwhZbDyYaUajzkpIap23ece+S
KvP3dho/nPVlL4q4b3+iGa1XSUnL6AEZKR2/7qHIFw==
```

![Logic NAND](./assets/logic-nand-pnps.png)

### "NOT-AND" Design

The right design produces a stable output with rising/falling lag of 2/2. The design on the left is
smaller, and the varying lag characters can be relatively beneficial, although it can produce
unintended spikes.

```
eNrtmVGSgyAQRMO0PznDXiH/e5a9/0V2Y4xZEGYAJRhtKatS9RhphqRrzAy34ev6
467fbrjUDAYWB8o4igPdPIoCxRtHzarUZdV5ozqr4pGqPQYKSpLjKdj3OVZKDY6o
VOq86ickR+qT48oCg28wnZyBDDxC4FjOSfoaKYDovZ7+cXnMmT55684UrxkJOs2I
0diOXnGCKJ1nqFQ2pw8wXOJ4ir9jxLEQr8VYhZMPD850U37/KRsTRF9g11hKaUvD
ShlllpOSkpKSnpse3SqTRaf8K+L2pRmm5nihHF7Q10Wf/U6bS8eikypjXdA6aJVH
NkNosci3nTeaIcTW7EuPrwvLSNHDDGE9GY1MSTVDXdUz2bQOWiXrRtaNrBtZN5Ke
+AVcr9/S3ZeOmnVVSPeiFt5gWEeX/cIyUqCTKuiURkqrbNwgfza+9Ra4qBRhqZXX
As+j726BW7Uu7Eq4vGNIqlIwG59F2/S4N7HK+L2eJv+f81QZdVRYaWUlZOmhe3h5
z1NFSnpu2tyRltcvu1nIPg==
```

![Logic NAND (NOT-AND)](./assets/logic-nand-notand.png)

## OR Gate

Output is high if any of the inputs are high, else output is low.

### NPN Design

By using multiple NPN gates (one for every 2 inputs) with a shared output, we create an OR gate
with a low rising/falling lag of 1/1.

```
eNrtmVsSgjAMRWnSH9bgFvx3Le5/I/LSKSVJKdiZQi+IM8zx0kfsNTX+6R/92/Uv
57sjJ4TVCl10ZrZIg4SW98yuHmwRccwWumNCIaqFW0QcjRkVVktaqKzPgi0ijhBC
WL9wSudIPybKzOJ1ng58fI33vuP5Nmj4h3mSaHT5gEqFIaUopSiF3QEFBbVosDq3
NJbvoCUtSbPCXV7ZJuXUF+C2s8FNjTeIM9YCKKwSFBQUFFaZTTmlPbsBv27eyHaW
db2cky0axll+MnJO0NazSnuLfecNODe1Abe32NiAg8IqraxyXQoSssq53KQaqaW9
9lzx7azSGlEY51wtjAVWuZb/ochN3wq2XKcmk7KS7RSvcduTiSonKOjOP6PqqYAX
tkr5Ok+ViY66vUn/oj5HCSJ+DUFBa6KJ9Zv/5OKOtD0+NePHHw==
```

![Logic OR](./assets/logic-or-npns.png)

### "NOT-NOR" Design

Using an inverter on a typical NOR gate results with fairly high rising/falling lag of 2/2.

```
eNrtmWsOgyAQhAvjH8/QK/R/z9L7X6QvUossDwVEZSQmTT7HArsdljLchuv4UONd
DZc1jcKthMq0hUL919Ra4bsxHBRWFEZTWxYmpHZYGEjtk8yqypsctVYYnVn+Oiik
sLzwU85p//WhAMQ7n764/j5jPlnf+6OYnvBQ84REpRFNZMad2QBpXWoCcLAR2fnI
+G5MazqSzwmTrJKUlJS0b9q1VfprTnlBY/IUp04AnBjtsc+I9QqML63yRGZYYAPO
1MozQ8jc2uruzQwhj8p+Mxh9WuXJrJJ1Y2OrPFzdCNaNtMrOJgRhI4XLmTyFKcJG
mrDVbdLnkJFC5Ix+H1ZZ4Ixbh8+4dZBivqtJO+MuMl08bSQl3Rutc8ZdxCrlO5+m
/R8Vqe7mC/miegZcSRvX9occERjBlrS6I7nXEz9Ax14=
```

![Logic OR (NOT-NOR)](./assets/logic-or-notnor.png)

## NOR Gate

Output is low if any of the inputs are high, else output is high.

```
eNrtmlsOgyAQRcsMP66hW+h/19L9b6RWNCKv4oN+lAMhMR4vwgSvmNE+7H14meFp
7O1IRfgroZnrTqF4lagiRIgQIUKEfyuctnOSLxNV1WQ7T8d9xnjoTsjS1huvWNdL
PCwena9I0c9M41k5Jn6vG7qUzqgLOeGAXk5VCzRQV9CGtpS1wyq/hEKh0L5p11ap
wcuO5QGFQru0yqIZVnyBs3igUGjvVskCgEKhWOVXqhgpFAq90CrPZZRc+jqT555T
1VKk6n8xxzRjd1oVEDKVUGhruj/HXaZtctyXWGW6nafpOIfDjuxwO+bgd6G6gMQO
y5sUCm1Di8/vgZ6bO1Jc3ivWxtw=
```

![Logic NOR](./assets/logic-nor.png)

## XOR Gate

Output is high if only an odd number of inputs are high, else output is low. For a 2-input XOR, it
is only high while only one input is high.

```
eNrtml0WgiAQhYXhxTW0hd5bS/vfSDWmcWwYQaX4uXHw5esKjXQdHN3VXca7GW/G
DXsahMULLR9NqtBws9yShJNkkidO1XgTxnUsUCispRihuJZihOJaipuqsJZwHSGE
EMLGhZzO2fCHKRGJ/Th98nefj/64p1Di0YJU+r2TiNbKhbph/oaI7TxwkH5NuSb6
iZpAvbAkU/3MDUayE7r5T7E2mea0pJAVRnklKCgoaN8UVqlmhntpt5EMZoYRFJEE
hVVWaIavrDy8rdBpy0aq2p0XlmQKIwWFVVaZN+bTNpw35tOCgsIqi6T8sHcn7TaS
XliSKSIJWr1VFl7k1mmoyL25Ader2A3XuHW6UQFfwoIaN6hETqF5atynWKXcj9Mf
3B3WbypEaVlE6pkJ91mJ0gGKSDb5mIvO33/9wZEecvfHLQ==
```

![Logic XOR](./assets/logic-xor.png)

### Compact Design

Smaller design, but can produce spikes in certain situations. Not recommended unless going for
low design score.

```
eNrtmk0WgjAMhCXDxjN4BfeexftfRJ/if9qURGiBgYebz6FpaMeU2h/7w/7c7U9d
v/OcFI4Uik/YDaerRbFbTbUo3uQIB0C5UHxCZVCUt/g1KMa0KN7kyHKe47zJCT2O
bsYhx4lMIYVtC2/lnKSPGwWgXnF65cP1+Hxvd6D3I0n1mFXdGx2+kabKjeUjV6hM
nwG6KLz0lZeWsmFEFehvKM9tjpx5qTEHs7MMFRwp5YRFVrlVCmZDpWBUpJujK7dK
VNK2TlFJyx6R0ipbNEMYlWF2Ab7smjM7/WHUYEBWW6u6C0Rl9Ag0UtJNW6VJsWAz
jFRKFkWTS124Y45kg9ZBuv4FONKbPnZFmtcuOlfQNyPKKtK8lj0i3bBVTr7Hnafp
Pe4sTfjd395GrngHvMn+GtmQQH+5xz0hja37pnCkSa1Sv+K0KOzf//wUabWycExF
yl9S37tKRkX6Wa78/84VHOkC2inHOw==
```

![Logic XOR Compact](./assets/logic-xor-compact.png)

### 4-Input XOR Gate

A 4-input XOR can be achieved with three 2-input XOR gates.

```
eNrtmVsagiAQhYXxxTW0hd5bS/vfSIWSqMM4in6IHI2Ifo8XGk8jtM/20b1N9zJt
s2ctVGiYVX1EqXUfoQ0kv3fL72IpNE5sncDM2oKw38T/FGbWFgPADDvwn8O2OnLM
3pCDcEWojJyGiSNV5MzXDZHTCJFUvstBCCGE1QldOmfji6NExJZ0+uX+Ndb/49rw
20tRcstYb6FujxTUUzpsMakPpP7MWBrvjQNopDdU1MrnHL9e0IJo2+jxmZ4U80KV
WYKCgoLWTWGV+2hKxlprT6ZkrIg60Nqtkoo0w1/K3pO+3kJvbKTyIzjfGyoKIwVF
VulvAboY9cOo0k1Kos3u05ZMUwwNZggKqxSzSr8U1ZluJNiPEMeo5WmlgUdyb6Cv
QG9glTXOcq/NgU8Lo802yy3S1DHDpDnw1bl3zAmDqug5c9yHWCVf0mm5/zu0fCZV
04xXNOTvefI3SqDIdkCzOtIHZDLHzQ==
```

![Logic XOR 4-Input](./assets/logic-xor-4.png)

## XNOR Gate

Output is low if only an odd number of inputs are high, else output is high. For a 2-input XNOR, it
is only high while all or none inputs are high.

```
eNrtmkESwiAMRaVh0zN4BfeexftfRKfiyGhIgRZh7CuDm+dvaRo/Qeov/jzf3Hx1
/lTTEA4vdN7VCKfQioUutIqhZlyPBDiWUMmkHKGavTlCNXvzhqpkL88RIUKEPxUu
5dyUPhYqImrfTh889NdnfN0d6PNIUv1+VV1EwxfSdLLpx3iPQ99RUWgU0mJqn5mn
MC5d+R11cKSUE2ZZJRQKhR6bYpXGfFdPiWQFTVSGWZRIQrHKTmYo5sJB1pYVpFap
3UUhLaYYKRSr7FY3ttNilT/WQqFYZTMqds2JVe5Nxa45sUro+FY59B63TdN73KsL
cPa4R9oBZ4/7P6nYa7cmjtTUKvW+nTafHb7f+cnSakUj8ywUOsafYB0c6Q57gMcH
```

![Logic XNOR](./assets/logic-xnor.png)

### 4-Input XNOR Gate

A 4-input XNOR can be achieved with three 2-input XNOR gates.

```
eNrtmUESgyAMRUvCxjP0Ct33LL3/RaoOOKghougg+GWcio+UIuE3Evux7+5nuq+x
ryOlUkMSS3KPpNRgeNzQWDMzDOuqYTh/0flcGxpXwv6FPiWXC7+fFvVkX6WjTg7D
DcNEz5H9iPZrzg7P0Typdl2FIQxhWNhwDOcofoyUmcUzn/acekUbbwQXU8/kb9vX
/Or8FuS63uK0iWkvZTdsFoevU/J3ZTo+4NnnLuoPic49SR72cvin09iPS6EDnqZS
XAbAEu4nuzz3LdIaXKlgMeVMklZQUFDQZ1NIZQGaEbA+9knmxLHwOtAGpJKfJ4bs
Rs3ie7JOGxZS/cU8tqeQQCGkoI1ElbzYXmuAut1IdZGyKrPHbGumOYIGMQRtP6pc
pRqanwghrbOmxFj+oRRuJYPwrEBvIJXZOfEhZvCxw8l7dxXSkilwlebvChbKjJNO
9fGC1kevyXGfIpXymU9jKxj/aCWoi+4xC6A3p5cr0vr4A+szyDU=
```

![Logic XNOR 4-Input](./assets/logic-xnor-4.png)
