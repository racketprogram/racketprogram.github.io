---
layout: post
title: Mod hash function
---

In the general situation, we choose the power of 2 to be the divider, because the mod operation can be reduced to follows.

```
h(k) = k & (n - 1)
```

But that is not a good choice when the inputs are pseudo-random. For example, an arithmetic progression that all least n bit number was the same, so hashed results are the same too.

```
n = 256

inputs = [1000, 2000, 3000, ..., 10000]

hash mapping = [0, 0, 0, ..., 0]
```
