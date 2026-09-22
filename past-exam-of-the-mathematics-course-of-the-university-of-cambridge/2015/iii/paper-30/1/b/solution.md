<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The increasing [quadratic variation](../../../../../../quadratic-variation.md) has a limit in $[0,\infty]$. Since $X_t$ has a finite limit, the exponentials have limits too, with value zero when the bracket is infinite. Expanding exponents proves

$$
\mathcal E(X)_t
=\mathcal E(rX)_t^{1/r^2}
\left(e^{rX_t/(r+1)}\right)^{(r^2-1)/r^2},
$$

because the coefficient of $X_t$ on the right is

$$
\frac1r+\frac{r}{r+1}\frac{r^2-1}{r^2}=1
$$

and the bracket coefficient is $-1/2$. Taking limits preserves the identity, including the zero case.

Let $A=\mathbb E[\mathcal E(X)_\infty]$, $B=\mathbb E[\mathcal E(rX)_\infty]$, and $D=\mathbb E[e^{rX_\infty/2}]$. The [Holder inequality](../../../../../../holder-inequality.md) first yields

$$
A\leq B^{1/r^2}
\left(\mathbb E[e^{rX_\infty/(r+1)}]\right)^{(r^2-1)/r^2}.
$$

When $D$ is finite, apply the [Jensen inequality](../../../../../../jensen-s-inequality.md) to the concave function $z\mapsto z^{2/(r+1)}$:

$$
\mathbb E[e^{rX_\infty/(r+1)}]
=\mathbb E[(e^{rX_\infty/2})^{2/(r+1)}]
\leq D^{2/(r+1)}.
$$

Since $D>0$, rearrangement gives the [terminal scaling inequality for stochastic exponentials](../../../../../../terminal-scaling-inequality-for-stochastic-exponentials.md)

$$
\boxed{
\mathbb E[\mathcal E(rX)_\infty]
\geq
\bigl(\mathbb E[\mathcal E(X)_\infty]\bigr)^{r^2}
\bigl(\mathbb E[e^{rX_\infty/2}]\bigr)^{-2(r-1)}.}
$$

Here $2(r^2-1)/(r+1)=2(r-1)$. If the last exponential moment is infinite, the bound has no positive content; the finite-moment form is the one used below.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
