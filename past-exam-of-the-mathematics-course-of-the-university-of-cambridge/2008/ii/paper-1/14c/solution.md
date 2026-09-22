<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

The chain rule gives $z_x=\sin2x$, $z_x^2=4z(1-z)$, and $z_{xx}=2(1-2z)$. Therefore

$$
4z(1-z)w_{zz}+2(1-2z)w_z+n^2w=0,
$$

which, after division, is the printed equation. It has only three [regular singular points](../../../../../regular-singular-point.md), $0,1,\infty$, and is thus a Papperitz equation. At zero and one the indicial roots are $0,1/2$. At infinity, inserting $w\sim z^{-\rho}$ gives $\rho=\pm n/2$. Its [Papperitz symbol](../../../../../papperitz-symbol.md) is

$$
\boxed{P\left\{\begin{matrix}0&\infty&1\\0&n/2&0\\1/2&-n/2&1/2\end{matrix};z\right\}.}
$$

The exponent sum is one, as required for a three-singularity second-order equation.

Multiplying the equation by $z(1-z)$ puts it in [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md) form with $a=n/2$, $b=-n/2$, $c=1/2$. The solution analytic at zero and normalized to one is ${}_2F_1(a,b;c;z)$. Composing it with $z=\sin^2x$ gives an even analytic solution of $w_{xx}+n^2w=0$ with $w(0)=1$, $w_x(0)=0$. Uniqueness of this [ordinary differential equation](../../../../../ordinary-differential-equation.md) implies

$$
\boxed{{}_2F_1(n/2,-n/2;1/2;\sin^2x)=\cos nx.}
$$

This [Gauss hypergeometric function](../../../../../hypergeometric-function.md) identity initially holds near zero, and on $|x|<\pi/2$ with the usual real branch; it extends by matching [analytic continuation](../../../../../analytic-continuation.md). It is not an identity on every real $x$ if the left side is always reevaluated on its principal $z$ branch: for $n=1$ that principal value is $\sqrt{1-\sin^2x}=|\cos x|$. Continuing the branch consistently restores the stated cosine.

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
