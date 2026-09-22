<h1 id="31j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The set $C$ is the [second-order cone](../../../../../../second-order-cone.md). Put

$$
\rho=\|u\|_2,
\qquad
\alpha=\frac12\left(1+\frac t\rho\right).
$$

When $\rho\geq|t|$ and $\rho>0$, one has $0\leq\alpha\leq1$, and the proposed point

$$
\pi=\alpha(u,\rho)
$$

lies on the boundary of $C$ because $\|\alpha u\|_2=\alpha\rho$.

Set $\delta=(\rho-t)/2\geq0$. Since

$$
(u,t)-\pi=\delta\left(\frac u\rho,-1\right),
$$

for any $(v,s)\in C$ we obtain

$$
\begin{aligned}
\bigl((u,t)-\pi\bigr)^T\bigl((v,s)-\pi\bigr)
&=\delta\left(\frac{u^Tv}{\rho}-s\right)\\
&\leq\delta(\|v\|_2-s)\\
&\leq0,
\end{aligned}
$$

where the first inequality is the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the second uses $\|v\|_2\leq s$. Part (d) therefore gives

$$
\boxed{
\pi_C(u,t)
=\frac12\left(1+\frac t{\|u\|_2}\right)
\bigl(u,\|u\|_2\bigr)
}
$$

whenever $\|u\|_2\geq|t|$ and $u\ne0$. At $(u,t)=(0,0)$ the projection is plainly $(0,0)$, consistent with the limiting formula.

If $\rho\leq-t$, then for every $(v,s)\in C$,

$$
(u,t)^T(v,s)
\leq\rho\|v\|_2+ts
\leq(\rho+t)s
\leq0.
$$

Applying part (d) with $\pi=0$ gives

$$
\boxed{\pi_C(u,t)=(0,0)}.
$$

Together with the trivial case $\rho\leq t$, this is the full [projection onto the second-order cone](../../../../../../projection-onto-the-second-order-cone.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [31J](../../31j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
