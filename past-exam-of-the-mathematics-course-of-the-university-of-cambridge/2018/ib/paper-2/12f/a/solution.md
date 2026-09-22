<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A map $f:A\to\mathbb R$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) with [Lipschitz constant](../../../../../../lipschitz-constant.md) $L$ when

$$
|f(y)-f(z)|\leq Ld(y,z)
$$

for all $y,z\in A$.

Fix $y_0\in A$. The Lipschitz inequality and the [triangle inequality](../../../../../../triangle-inequality.md) imply

$$
f(y)+Ld(x,y)\geq f(y_0)-Ld(y,y_0)+Ld(x,y)
\geq f(y_0)-Ld(x,y_0),
$$

while choosing $y=y_0$ gives a finite upper bound. Hence the [infimum](../../../../../../infimum.md) defining $F(x)$ is a real number.

If $x\in A$, then $f(x)\leq f(y)+Ld(x,y)$ for every $y\in A$, while $y=x$ gives the reverse inequality after taking the infimum. Thus $F(x)=f(x)$. For arbitrary $x,z\in X$,

$$
f(y)+Ld(x,y)\leq f(y)+Ld(z,y)+Ld(x,z).
$$

Taking infima gives $F(x)\leq F(z)+Ld(x,z)$; interchanging $x,z$ gives

$$
\boxed{|F(x)-F(z)|\leq Ld(x,z).}
$$

This is the [McShane extension theorem](../../../../../../mcshane-extension-theorem.md): **$F$ extends $f$ without increasing its Lipschitz constant.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
