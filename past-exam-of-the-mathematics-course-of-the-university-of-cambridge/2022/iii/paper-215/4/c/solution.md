<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose vertices $x,y$ at distance $d_G$, put $r=\lfloor(d_G-1)/4\rfloor$ and $R=\lfloor(d_G-1)/2\rfloor$. The radius-$R$ balls about $x$ and $y$ are disjoint, so one has stationary mass at most $1/2$; call its center $z$. Apply part b from radius $r$ to radius $R$:

$$
\frac12\geq\pi^G(B(z,R))
\geq\pi_*^G(1+\Phi_*^G)^{R-r}.
$$

Here the exponent should be $R-r$, and $R-r\geq(d_G-2)/4$. Therefore

$$
\Phi_*^G
\leq(2\pi_*^G)^{-4/(d_G-2)}-1.
$$

Since the [relaxation time](../../../../../../relaxation-time.md) is $t_{\rm rel}^G=1/\gamma^G$, part a yields

$$
\boxed{t_{\rm rel}^G
\geq
\frac1{2\Phi_*^G}
\geq
\frac1{2\{(2\pi_*^G)^{-4/(d_G-2)}-1\}}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
