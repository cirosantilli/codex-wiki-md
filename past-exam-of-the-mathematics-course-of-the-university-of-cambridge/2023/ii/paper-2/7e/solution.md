<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For $\Re s>1$, absolute convergence permits separation into odd and even terms:

$$
\begin{aligned}
\sum_{n=1}^\infty(-1)^{n-1}n^{-s}
&=\sum_{n=1}^\infty n^{-s}-2\sum_{n=1}^\infty(2n)^{-s}\\
&=(1-2^{1-s})\zeta(s).
\end{aligned}
$$

Using the defining integral of the [Gamma function](../../../../../gamma-function.md) and the substitution $u=nt$ gives

$$
\Gamma(s)n^{-s}=\int_0^\infty t^{s-1}e^{-nt}\,dt.
$$

Termwise integration is justified by absolute convergence when $\Re s>1$, and the geometric sum is

$$
\sum_{n=1}^\infty(-1)^{n-1}e^{-nt}=\frac1{1+e^t}.
$$

Consequently the [Dirichlet eta function](../../../../../dirichlet-eta-function.md) satisfies

$$
(1-2^{1-s})\zeta(s)=\eta(s)
=\frac1{\Gamma(s)}\int_0^\infty\frac{t^{s-1}}{1+e^t}\,dt.
$$

Near zero the integrand is $O(t^{\Re s-1})$, while at infinity it decays exponentially. The integral therefore defines a holomorphic function for $\Re s>0$. Thus

$$
\boxed{\displaystyle
\zeta(s)=\frac1{(1-2^{1-s})\Gamma(s)}
\int_0^\infty\frac{t^{s-1}}{1+e^t}\,dt}
$$

provides the desired continuation wherever the displayed denominator is nonzero. At a nonreal zero of $1-2^{1-s}$, use instead

$$
(1-k^{1-s})\zeta(s)
=\sum_{n\geq1}a_n n^{-s},
\qquad
a_n=\begin{cases}1,&k\nmid n,\\1-k,&k\mid n,
\end{cases}
$$

with an integer $k$ for which $1-k^{1-s}\ne0$; the bounded partial sums of $a_n$ give convergence for $\Re s>0$. This shows that those apparent singularities are removable and yields the [Analytic continuation of the Riemann zeta function to the right half-plane](../../../../../analytic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane.md).

At $s=1$,

$$
\eta(1)=\int_0^\infty\frac{dt}{1+e^t}=\log2,
$$

whereas

$$
1-2^{1-s}=1-e^{-(s-1)\log2}
=(s-1)\log2+O((s-1)^2).
$$

Hence

$$
\zeta(s)=\frac1{s-1}+O(1),
$$

so $s=1$ is a simple pole and its [residue](../../../../../residue.md) is

$$
\boxed{\operatorname{Res}_{s=1}\zeta(s)=1}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
