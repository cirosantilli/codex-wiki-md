<h1 id="b/4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

From $B_kp_k=-g_k$ and the [matrix 2-norm](../../../../../matrix-2-norm.md) bound, $\|g_k\|_2\leq\kappa_b\|p_k\|_2$, so $\|p_k\|_2\geq\|g_k\|_2/\kappa_b$. Let $C=2\tau\varepsilon(1-\beta)/\gamma>0$. The summand in the supplied decrease bound satisfies

$$
\min\left(\alpha_{\mathrm{init}},C\frac{\|g_k\|_2}{\|p_k\|_2}\right)\|g_k\|_2\|p_k\|_2
=\min\left(\alpha_{\mathrm{init}}\|g_k\|_2\|p_k\|_2,C\|g_k\|_2^2\right)
\geq\min(\alpha_{\mathrm{init}}/\kappa_b,C)\|g_k\|_2^2.
$$

Thus, with the fixed positive constant $c=\beta\varepsilon\min(\alpha_{\mathrm{init}}/\kappa_b,C)$,

$$
c\sum_{k=0}^j\|g_k\|_2^2\leq f(x_0)-f(x_{j+1})\leq f(x_0)-\inf f<\infty.
$$

The nonnegative series therefore converges, forcing its terms to zero:

$$
\boxed{\lim_{k\to\infty}g(x_k)=0.}
$$

The argument uses the given angle condition and upper bound on $\|B_k\|_2$; it does not need an additional uniform lower eigenvalue bound on $B_k$.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
