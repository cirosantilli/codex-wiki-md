<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [canonical coordinates](../../../../../canonical-variables.md), the [Poisson bracket](../../../../../poisson-bracket.md) is

$$
\boxed{\{f,g\}=\sum_i\left(\frac{\partial f}{\partial q_i}\frac{\partial g}{\partial p_i}
-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q_i}\right).}
$$

In particular, $\{q_j,g\}=\partial_{p_j}g$, $\{p_j,g\}=-\partial_{q_j}g$, $\{f,q_j\}=-\partial_{p_j}f$ and $\{f,p_j\}=\partial_{q_j}f$. Hence $\{q_i,p_j\}=\delta_{ij}$ and the coordinate–coordinate and [momentum](../../../../../momentum-split.md)–[momentum](../../../../../momentum-split.md) brackets vanish.

The [chain rule](../../../../../chain-rule.md) along a [Hamiltonian](../../../../../hamiltonian.md) trajectory gives

$$
\frac{df}{dt}=\partial_tf+\sum_i(\partial_{q_i}f\,\dot q_i+\partial_{p_i}f\,\dot p_i)
=\boxed{\partial_tf+\{f,H\}.}
$$

The [Poisson bracket of time-dependent conserved quantities](../../../../../poisson-bracket-of-time-dependent-conserved-quantities.md) follows by defining $D_t=\partial_t+\{\,\cdot\,,H\}$. The ordinary [product rule](../../../../../product-rule.md) and [Jacobi identity](../../../../../jacobi-identity.md) imply

$$
D_t\{f,g\}=\{D_tf,g\}+\{f,D_tg\}.
$$

To see the [Hamiltonian](../../../../../hamiltonian.md) part explicitly, Jacobi rearranges to $\{\{f,g\},H\}=\{\{f,H\},g\}+\{f,\{g,H\}\}$. Therefore $D_tf=D_tg=0$ implies **$D_t\{f,g\}=0$**, even when the conserved functions depend explicitly on time.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
