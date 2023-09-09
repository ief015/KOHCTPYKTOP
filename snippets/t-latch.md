# T Latches

This T-Latch comes in two flavours:

a) Larger but very accurate. Rising/falling lag of 0/1.

b) Slightly smaller but less accurate. Rising/falling lag of 1/1.

```
eNrtWlF2gzAMKxE/O8OusP+dZfe/yPpYVxxjK+CkQNtA+7EKE8cxQrE3fo2fHz/D
x/cwXiJnNzy54RAzTPdzo+FwO0Ouhka8xEfsmXMaQ3aTwTdkebr4XRqyPF1g2lU/
TxWmDf08pSM+1ToG5xiMangdw5kTztWj17FAk8yQErNnOERHLL4GmKudVyc5l/xj
QgGY33r0ik+f/wOQ42o07YgCuDuzQDNQo7cLfDSbsIGKY4GOF2+R+BLebiwj/ffX
jKp4wLdN2paOi+xXK5T6vsLWGlaifEbGwCvRQiTjd+Y+0/mWYsXiXJrR7I7MMA1f
Pz6cu6celgmz0NnQQ+eLdiMlL1qr2LKjHe1oR98b7VTpoVBval8cWneusX0nFEze
F9WfBTdRjjXow3wuxOrRKwhui7AtOlWenwxpwhtcKVOakSGY7duRYaK1jgS98ffq
M5pY8ihDlw3OGQ3mM58vj1WLLXgFqjM+Q0GJFE9CpJ0qfe0XV4bgtp0qZR20pvJH
apnHkSH1qlDpBFWVx5JhXDd2VfnKKCjdWeBqmkXfgMuyfyZNNGo9qx6xLDTnEtxH
N7Jxmc98vjxWe+hGSoZMN1JbvBJVNm1z64flsDZ3AU28zZ0YWmpzH6INzFKXq3aa
bWZrVKXZmN+jy11TjdxUb8SZVKXdiV6F6nqVeI58W9njdlGTNx7T425Clfa3HtUH
zqMqSTXSKkWmDW2d0sZf/7tQK50c365S/VajKulrtEgOtEXyFGUfbKnr0li1oEog
Pl94uwbjacmzveyzvGhnRrofv0gYyIo=
```

![T LATCH](./assets/t-latch.png)

## T Latch in use with simplified variant

On the left shows a simplified implementation of a T-Latch. At it's core, it is a simple
SR-Latch, with both S+R inputs connected, forming T. R is only available when the output is high.
There is a major problem with this approach: the latch will oscillate while T is high, as S will
allow R to open. To combat this, we add a PNP gate in order to trigger T with a short pulse so that
R does not receive a high signal, as it's NPN hasn't had enough time to open.

```
eNrtmlF6gyAQhAPjS87QK/S9Z+n9L9IW0WiAXbOIQTv6+ZKfYRMc9lsgw+fwcf92
9y833Cz3yYXeLnQHR1zKnV3oD4rowu3D/XJEbxNe26sUUkihLnQ2oZBxJKGbb9NX
LUbVhMaIdM71haGc8+UrUADZp57+8vEZbmM8rAJHDBlr6nD9NcphH2ZUbJfl05XQ
2PH4g56pNJ6k88CX+cLbQov/MGaQ6MJ5qTeBNZ5otHxsl/I5cLbvBy3Mmcfnlvmq
4ux8bJmjSu9pU/J8L0XjuGByIyUlPX+q7JaCaZa0t7pT9SRYNpw4VSp1I6pqTtSZ
p9zzuBintUgPXoRLfobi57Vl+RaulSorF+ByqqykTJWkvdWNIs3uZvItXGQB3ute
5XjGU06kAJczpPtTSIlUdR2UmpPjXJUqdzn1fk5Mm6lvprVSmoe0twU4sivsl0+5
RWqbgy1omzPuXVJl/qmnravK5A8U2b3KRYtNPU+9wqAlJa2sKgVPQl2812wZoeD2
ZI41H403ZKQfNXDHag==
```

![T LATCH - usage](./assets/t-latch-usage.png)

## See Also

[07 KL2T1 DUAL TOGGLE LATCH](/levels/07%20KL2T1%20DUAL%20TOGGLE%20LATCH.md)
