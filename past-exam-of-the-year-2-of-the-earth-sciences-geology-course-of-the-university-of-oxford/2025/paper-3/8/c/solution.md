<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [separation of variables](../../../../../separation-of-variables.md) with a nontrivial product $\eta=XT$. Substitution into the [wave equation on a string](../../../../../wave-equation-on-a-string.md) gives $\tau_0X''T=\lambda_0XT''$. Wherever the factors are nonzero,

$$
\frac{X''(x)}{X(x)}=\frac{\lambda_0}{\tau_0}\frac{T''(t)}{T(t)}.
$$

The left side depends only on $x$ and the right only on $t$, so both are a constant. For nontrivial fixed-end solutions this constant is negative: multiplying $X''=\sigma X$ by $X$ and integrating, using the homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), gives

$$
\sigma\int_0^LX^2\,dx=-\int_0^L(X')^2\,dx<0.
$$

Write it as $-k^2$. The separated equations are therefore

$$
\boxed{X''+k^2X=0,\qquad T''+c^2k^2T=0.}
$$

These equations extend across the zeros of $X$ and $T$; the division is a derivation device, not a restriction excluding their nodes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
