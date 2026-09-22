# Automatic continuity onto a semisimple Banach algebra

↑ **Parent:** [Semisimple Banach algebra](semisimple-banach-algebra.md)

An [algebra homomorphism](algebra-homomorphism-over-a-field.md) onto a [semisimple Banach algebra](semisimple-banach-algebra.md) is [continuous](continuous-function.md). To see the spectral mechanism, suppose $a_n\to0$ and $T(a_n)\to b$. For any $c\in B$, choose $u,v\in A$ with $T(u)=b$ and $T(v)=c$, and [set](set-split.md) $d=cb$, $d_n=T(va_n)$. Apply the [spectral-radius three-circle inequality](spectral-radius-three-circle-inequality.md) to $T((1-z)va_n+zvu)$. On the outer circle its [norm](norm.md) tends uniformly to $\|d\|$; on the circle of radius $1/R$ its [spectral radius](spectral-radius.md) is bounded by $(1+1/R)\|va_n\|+\|vu\|/R$. Hence $r(d)^2\le\|d\|\|vu\|/R$ for every $R>1$, so $r(cb)=0$. The [unit criterion for the Jacobson radical](unit-criterion-for-the-jacobson-radical.md) gives $b\in J(B)=0$, and the [closed graph theorem](closed-graph-theorem.md) finishes the proof.

## ↑ Ancestors (7)

1. [Semisimple Banach algebra](semisimple-banach-algebra.md)
2. [Banach algebra](banach-algebra-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
