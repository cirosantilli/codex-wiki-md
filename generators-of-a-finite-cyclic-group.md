# Generators of a finite cyclic group

↑ **Parent:** [Generator of a group](generator-of-a-group.md)

An element $k$ of the additive [finite cyclic group](finite-cyclic-group.md) $C_n=\mathbb Z/n\mathbb Z$ is a [generator of a group](generator-of-a-group.md) precisely when $\gcd(n,k)=1$. The [order of an element of a finite cyclic group](order-of-an-element-of-a-finite-cyclic-group.md) proves this immediately: its [cyclic subgroup](cyclic-subgroup.md) has size $n/\gcd(n,k)$, and this equals $n$ exactly when the [greatest common divisor](greatest-common-divisor.md) is one. There are therefore $\varphi(n)$ choices, where $\varphi$ is the [Euler totient function](euler-totient-function.md).

For $C_6$, the two choices are $1$ and $5$, so $\varphi(6)=2$. For $C_8$, they are $1,3,5,7$. Starting from zero and repeatedly adding $3$ modulo eight gives $0,3,6,1,4,7,2,5,0$, visiting every element once before returning. By contrast, adding $2$ gives $0,2,4,6,0$ and misses the [odd integers](odd-integer.md) represented in the other [coset](coset.md).

If the [cyclic group](cyclic-group.md) is written multiplicatively as $\langle g\rangle$ with $g$ of order $n$, the same statement says that $g^k$ is a [generator of a group](generator-of-a-group.md) exactly when $k$ and $n$ are [coprime](coprime-integers.md). This changes notation without changing the calculation.

## ↑ Ancestors (8)

1. [Generator of a group](generator-of-a-group.md)
2. [Cyclic group](cyclic-group.md)
3. [Group](group-split.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Endomorphism of a finite cyclic group](endomorphism-of-a-finite-cyclic-group.md)
- [Finite cyclic group](finite-cyclic-group.md)
- [Group automorphism](group-automorphism.md)
