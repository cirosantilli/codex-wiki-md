<h1 id="b/8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $x=B^2/S$ and $q=(S/B)^\alpha$, so $W=qV(t,x)$. Direct differentiation gives

$$
W_t=qV_t,\qquad SW_S=q(\alpha V-xV_x),
$$



$$
S^2W_{SS}=q\left[\alpha(\alpha-1)V+
2(1-\alpha)xV_x+x^2V_{xx}\right].
$$

Substitute into the [Black-Scholes equation](../../../../../black-scholes-equation.md) and divide by $q$:

$$
\frac{\mathcal LW}{q}=V_t+\tfrac12\sigma^2x^2V_{xx}
+[\sigma^2(1-\alpha)-r]xV_x
+[\tfrac12\sigma^2\alpha(\alpha-1)+r\alpha-r]V.
$$

To recover the same operator on $V$, its first-derivative coefficient must be $r$. This gives

$$
\boxed{\alpha=1-\frac{2r}{\sigma^2}.}
$$

For this choice the last coefficient is $-r$, since $\tfrac12\sigma^2(\alpha-1)+r=0$. Hence $\mathcal LW=q\mathcal LV=0$, proving the required invariance. The transformation is the [stock-inversion reflection for the Black-Scholes equation](../../../../../stock-inversion-reflection-for-the-black-scholes-equation.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
