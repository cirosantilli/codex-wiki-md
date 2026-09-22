<h1 id="1/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [radial reduction of the three-dimensional wave equation](../../../../../../radial-reduction-of-the-three-dimensional-wave-equation.md) $w=r\phi$ and extend $w$ oddly in $r$. Write $w=w_h+w_F$, where $w_h$ is the homogeneous [wave equation](../../../../../../wave-equation-split.md) solution with the prescribed [Cauchy data](../../../../../../cauchy-data.md), and $w_F$ has zero [Cauchy data](../../../../../../cauchy-data.md). With $w_0(r)=r\phi_0(r)$ and $w_1(r)=r\phi_1(r)$, the [D'Alembert formula](../../../../../../d-alembert-s-formula.md) gives

$$
w_h(t,r)=\frac{w_0(r-t)+w_0(r+t)}2+\frac12\int_{r-t}^{r+t}w_1(\rho)\,d\rho.
$$

Both odd initial profiles have [compact support](../../../../../../compact-support.md), so

$$
|w_h(t,r)|\leq A,\qquad A=\|w_0\|_\infty+\frac12\|w_1\|_1.
$$

The [Duhamel principle](../../../../../../duhamel-s-principle.md), applied to $w_{tt}-w_{rr}=-rF$, gives

$$
w_F(t,r)=-\frac12\int_0^t\int_{r-(t-s)}^{r+(t-s)}\rho F(s,\rho)\,d\rho\,ds.
$$

Now write $r=t+a$ with $1/2\leq a\leq1$. The lower integration limit is $s+a>0$, so this [domain of dependence](../../../../../../domain-of-dependence.md) never crosses the axis. Intersecting its integration interval with the [support](../../../../../../support.md) of the source leaves a subset of $[s+a,s+1]$, of length at most one. On this interval,

$$
\rho |F(s,\rho)|\leq\frac{s+1}{(1+s)^2}=\frac1{1+s}.
$$

The [outgoing shell source estimate for a radial wave](../../../../../../outgoing-shell-source-estimate-for-a-radial-wave.md) therefore yields

$$
|w_F(t,t+a)|\leq\frac12\int_0^t\frac{ds}{1+s}=\frac12\log(1+t).
$$

Finally $r\geq t+1/2\geq(1+t)/2$, and thus

$$
|\phi(t,t+a)|\leq\frac{2A+\log(1+t)}{1+t}
\leq\boxed{\frac{C\log(2+t)}{1+t}},\qquad C=1+\frac{2A}{\log2}.
$$

This constant depends only on the [Cauchy data](../../../../../../cauchy-data.md) and the fixed unit bound for the source. The logarithm comes from integrating the shell's accumulated forcing, whereas the factor $(1+t)^{-1}$ comes from division by $r$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
