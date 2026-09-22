<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Von Mangoldt function](../../../../../../von-mangoldt-function.md) is supported on [prime powers](../../../../../../prime-power.md):

$$
\Lambda(n)=\begin{cases}\log p,&n=p^k\text{ for a prime }p,\ k\geq1,\\0,&\text{otherwise}.\end{cases}
$$

Write $e(t)=\exp(2\pi it)$. A convenient form of the [Siegel–Walfisz theorem](../../../../../../siegel-walfisz-theorem.md) is: for every fixed $A,B>0$, uniformly for $q\leq(\log x)^B$ and $(a,q)=1$,

$$
\psi(x;q,a):=\sum_{\substack{n\leq x\\n\equiv a\pmod q}}\Lambda(n)
=\frac{x}{\varphi(q)}+O_{A,B}\left(\frac{x}{(\log x)^A}\right).
$$

The implied constant can be ineffective because of possible [Siegel zeros](../../../../../../siegel-zero.md); the modulus bound is logarithmic, not an unrestricted uniformity assertion.

Apply this to modulus five and separate the reduced [residue classes](../../../../../../residue-class.md):

$$
\sum_{n\leq N}\Lambda(n)e(2n/5)
=\sum_{a=1}^4e(2a/5)\psi(N;5,a)
+\sum_{5^k\leq N}\log5.
$$

The last sum is $O(\log N)$: only powers of five can contribute in the zero [residue class](../../../../../../residue-class.md). By the [orthogonality of roots of unity](../../../../../../orthogonality-of-roots-of-unity.md),

$$
\sum_{a=1}^4e(2a/5)=-1,
$$

since two is coprime to five and the sum including $a=0$ vanishes. As $\varphi(5)=4$, the [Siegel–Walfisz theorem](../../../../../../siegel-walfisz-theorem.md) yields

$$
\boxed{\sum_{n\leq N}\Lambda(n)e(2n/5)
=-\frac N4+O_A\left(\frac{N}{(\log N)^A}+\log N\right)
\sim-\frac N4,\qquad c=-\frac14.}
$$

The sum is complex-valued, but the displayed error controls its absolute difference from the real main term.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7](../../7.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
