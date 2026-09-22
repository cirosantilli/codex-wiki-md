<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $v$ be the voltage with $v(a)=1$, $v(b)=0$, and harmonic values at every other vertex. For any other admissible $f$, write $f=v+g$, where $g(a)=g(b)=0$. Its [discrete Dirichlet energy](../../../../../../discrete-dirichlet-energy.md) expands as

$$
\mathcal E(f)=\mathcal E(v)+\mathcal E(g)
+\sum_{x,y}c(x,y)(v(x)-v(y))(g(x)-g(y)).
$$

Discrete summation by parts turns the cross term into

$$
2\sum_xg(x)\sum_yc(x,y)(v(x)-v(y))=0,
$$

because $v$ is harmonic in the interior and $g$ vanishes at the boundary. Thus $v$ minimizes the energy. Under a unit voltage drop, its energy equals the total current from $a$ to $b$, namely the [effective conductance](../../../../../../effective-conductance.md) $1/R_{\mathrm{eff}}(a,b)$. Therefore the [Dirichlet principle](../../../../../../dirichlet-principle.md) gives

$$
\boxed{
\frac1{R_{\mathrm{eff}}(a,b)}
=\inf_{f(a)=1,\,f(b)=0}
\frac12\sum_{x,y}(f(x)-f(y))^2c(x,y).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
