<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A(s)=\sum_{n\ge1}a_nn^{-s}$ converge absolutely at a real $c>0$, and take $T\ge\max(2,c)$. Define

$$
K_T(v)=\frac1{2\pi i}\int_{c-iT}^{c+iT}\frac{v^s}s\,ds.
$$

The [truncated Perron kernel estimate](../../../../../../truncated-perron-kernel-estimate.md) is

$$
K_T(v)=1_{v>1}+O\left(v^c\min\left(1,\frac1{T|\log v|}\right)\right)\quad(v\ne1),\qquad K_T(1)=\frac1\pi\arctan(T/c)=\frac12+O(c/T).
$$

For $v>1$ close the contour to the left, collecting the [residue](../../../../../../residue.md) one at zero; for $v<1$ close it to the right, collecting no [residue](../../../../../../residue.md). On the horizontal sides, integrating $v^\sigma$ bounds the error by $O(v^c/(T|\log v|))$, and the remote vertical side tends to zero. Near $v=1$ use the bounded transition estimate instead, giving $O(v^c)$. These are the contours and bounds underlying the kernel formula. The constants are uniform for $1\le c\le2$, the range needed below.

[Absolute convergence](../../../../../../absolute-convergence.md) permits termwise integration. The [truncated Perron formula](../../../../../../truncated-perron-formula.md) is consequently

$$
\sum_{n\le x}'a_n=\frac1{2\pi i}\int_{c-iT}^{c+iT}A(s)\frac{x^s}s\,ds+O\left(\sum_{n\ne x}|a_n|(x/n)^c\min\left(1,\frac1{T|\log(x/n)|}\right)+\frac{c|a_x|}T\right).
$$

Here the primed sum has half weight when $x$ is an integer, and $a_x=0$ otherwise. To obtain the inclusive sum add $a_x/2$ at an integer. This endpoint convention avoids a false uniform assertion about the kernel at $v=1$.

Apply this with $a_n=\Lambda(n)$, $A=-\zeta'/\zeta$, $c=1+1/\log x$ and $2\le T\le x$, for sufficiently large $x$. For $n\notin[x/2,2x]$, $|\log(x/n)|$ is bounded below, and

$$
\frac{x^c}T\sum_n\Lambda(n)n^{-c}\ll\frac{x\log x}T,
$$

using $-\zeta'(c)/\zeta(c)\ll(c-1)^{-1}$. In the central range $(x/n)^c\ll1$, $\Lambda(n)\ll\log x$, and $|\log(x/n)|\asymp|n-x|/x$. Separate the nearest integers, then sum the harmonic tail over distances $j\ge1$: its contribution is $O((x/T)\log^2x)$. The possible endpoint weight and nearest terms, of size $O(\log x)$, are absorbed because $T\le x$. Therefore

$$
\boxed{\psi(x)=\frac1{2\pi i}\int_{c-iT}^{c+iT}-\frac{\zeta'(s)}{\zeta(s)}\frac{x^s}s\,ds+O\left(\frac{x\log^2x}T\right).}
$$

For $x+y$, use the same vertical line $c=1+1/\log x$; the error estimate remains valid since $x\le x+y\le2x$. Subtract the two formulas. The identity

$$
\frac{(x+y)^s-x^s}s=\int_x^{x+y}u^{s-1}\,du
$$

has absolute value $O(y)$ on that line, because $(2x)^{c-1}$ is bounded. Taking absolute values gives

$$
\boxed{\psi(x+y)-\psi(x)\ll y\int_{-T}^T\left|\frac{\zeta'(c+it)}{\zeta(c+it)}\right|dt+\frac{x\log^2x}T,\qquad1\le y\le x.}
$$

This is the [short-interval Perron bound for the second Chebyshev function](../../../../../../short-interval-perron-bound-for-the-second-chebyshev-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
