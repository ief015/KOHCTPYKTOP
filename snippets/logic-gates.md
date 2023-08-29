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
characteristics and unintended side-effects similar to the 2-input single-NPN gate shown previously.

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

### 2-Input

The left design produces a stable output with rising/falling lag of 2/2. The design on the right is
smaller, and the varying lag characters can be beneficial, although it can produce unintended
side-effects.

```
eNrtml0SgjAMhIXlxTN4Bd89i/e/iAwyYNsklCK/WTodcD5jY5tuU2vzbB73d3V/
Vc2tpNBwpmHdlgLDqi+zDeuhcDgcG6YBUOcYpmGXhKFsKIVd9Pr0vVr8HYt7tXgc
OTsOaWgIs2VoLgVTLXI4rm7YpXO1fnUUgFiX05Z3Ff1T2G4WhUq/SKGjuULV3nBK
sYB68+pwFMMVRPzPPBrvaG4Kxp4YKV5Tl7T+zBJMUlJSUt/04lKJiewCDI9sCkSd
FtlGeDOfrXanfPY3vuZOCoz2C0ulKYYwbSG8g2KoCQuSh5j2u7j+vt02XG/X9tmj
kCKIeGXRoZD6k0rmjZfIG5lVMqukVK5LYeecAmZ4qPnbcFQGmUZ4M6+Mdm2fPY6v
eZQJSuVSqdz5pNuk5lqJjJWUYpi/1aVXJ6WQk0f5HFyj2ImG83/FM+6/SKVcl9M1
J4uUUiafDK6kpA6kcvjHUBDxZ/l99QiK9AEyr8dg
```

![Logic NAND 2-input](./assets/logic-nand-2.png)

### 4-Input

The right design produces a stable output with rising/falling lag of 2/2. The design on the left is
smaller, and the varying lag characters can be beneficial, although it can produce unintended
side-effects.

```
eNrtmV2OgzAMhBsPLz3DXmHf9yy9/0W6BQoFHOcHAikMEVKlL0Nc04ycuvltfu4P
d/9zzS1nUJgslHYkC90wkoQyGWfNquRl1U1GdlblG7M6CzxWuEhXWqgfq9abHMlL
jstNjvJboq9SSCGFOcK2nBP/1VIA6r2e/nPp5vSfJusOFOMMD+1naFT7RqNOoNJh
hkllc9qB5qbjXv/C0LEQYxUuFtrsnW7KX1s5MEHsBarGkkpLGpbPKKOclJSUlPTa
9OxW6S065aOIqytmBGPWC+XdYn7H59XigKhQZVSktMovMUNYWhxlO6YZQsIxmweW
0maI0JO7E9O+ZghTO75pbn9SWiXrRtaN3OCktMoC9Zu/+3JgzHZU8PeiqrEsHGBZ
sGvOAXP7k5a0yg1a4GK3wMWk8Bz9Ai3wOLp3CzxU6yJcCad3DE9PwWxciZbpcW9i
lfq9nnr/n5tEFaij5pVWVEKWHlrD4T0uKlLSa9PijrS8ntmzyCc=
```

![Logic NAND 4-input](./assets/logic-nand-4.png)

## OR Gate

Output is high if any of the inputs are high, else output is low.

### NPN Design

By using multiple NPN gates (one for every 2 inputs), with a shared output, we create an OR gate
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
eNrtmk0WgjAMhCXDxjN4BfeexftfRJ/if9qURGiBgYebz6FpaMeU2h/7w/7c7U9d
v/OcFI4Uik/YDaerRbFbTbUo3uQIB0C5UHxCZVCUt/g1KMa0KN7kyHKe47zJCT2O
bsYhx4lMIYVtC2/lnKSPGwWgXnF65cP1+Hxvd6D3I0n1mFXdGx2+kabKjeUjV6hM
nwG6KLz0lZeWsmFEFehvKM9tjpx5qTEHs7MMFRwp5YRFVrlVCmZDpWBUpJujK7dK
VNK2TlFJyx6R0ipbNEMYlWF2Ab7smjM7/WHUYEBWW6u6C0Rl9Ag0UtJNW6VJsWAz
jFRKFkWTS124Y45kg9ZBuv4FONKbPnZFmtcuOlfQNyPKKtK8lj0i3bBVTr7Hnafp
Pe4sTfjd395GrngHvMn+GtmQQH+5xz0hja37pnCkSa1Sv+K0KOzf//wUabWycExF
yl9S37tKRkX6Wa78/84VHOkC2inHOw==
```

![Logic XOR](./assets/logic-xor.png)

### Simplified Design

```
eNrtml0WgiAQhYXhxTW0hd5bS/vfSDWmcWwYQaX4uXHw5esKjXQdHN3VXca7GW/G
DXsahMULLR9NqtBws9yShJNkkidO1XgTxnUsUCispRihuJZihOJaipuqsJZwHSGE
EMLGhZzO2fCHKRGJ/Th98nefj/64p1Di0YJU+r2TiNbKhbph/oaI7TxwkH5NuSb6
iZpAvbAkU/3MDUayE7r5T7E2mea0pJAVRnklKCgoaN8UVqlmhntpt5EMZoYRFJEE
hVVWaIavrDy8rdBpy0aq2p0XlmQKIwWFVVaZN+bTNpw35tOCgsIqi6T8sHcn7TaS
XliSKSIJWr1VFl7k1mmoyL25Ader2A3XuHW6UQFfwoIaN6hETqF5atynWKXcj9Mf
3B3WbypEaVlE6pkJ91mJ0gGKSDb5mIvO33/9wZEecvfHLQ==
```

![Logic XOR Simplfied](./assets/logic-xor-simplified.png)

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
