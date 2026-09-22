<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the same [Minkowski metric](../../../../../minkowski-metric.md) and electromagnetic units, $T^{\mu\nu}=-F^\mu{}_{\lambda}F^{\nu\lambda}+\tfrac14g^{\mu\nu}F_{\alpha\beta}F^{\alpha\beta}$. Differentiating gives

$$
\partial_\mu T^{\mu\nu}=-(\partial_\mu F^\mu{}_{\lambda})F^{\nu\lambda}-F^\mu{}_{\lambda}\partial_\mu F^{\nu\lambda}+\frac14\partial^\nu(F_{\alpha\beta}F^{\alpha\beta}).
$$

To simplify the last two terms, contract $\partial_\mu F_{\nu\lambda}+\partial_\nu F_{\lambda\mu}+\partial_\lambda F_{\mu\nu}=0$ with $F^{\mu\lambda}$. Its first and third terms are equal, and its middle term is $-\tfrac12\partial_\nu(F_{\alpha\beta}F^{\alpha\beta})$. Raising $\nu$ therefore gives $F^\mu{}_{\lambda}\partial_\mu F^{\nu\lambda}=\tfrac14\partial^\nu(F_{\alpha\beta}F^{\alpha\beta})$. The cancellation leaves

$$
\partial_\mu T^{\mu\nu}=-F^{\nu\lambda}\partial_\mu F^\mu{}_{\lambda},\qquad \boxed{\partial_\mu T^{\mu\nu}=0\quad\text{in vacuum}.}
$$

This is the [electromagnetic stress-energy divergence identity](../../../../../electromagnetic-stress-energy-divergence-identity.md) in rationalized units. As a sign check, $T^{00}=(E^2+B^2)/2$ is positive and $T^{0i}=(\mathbf E\times\mathbf B)_i$ is the [Poynting vector](../../../../../poynting-vector.md). The integrated [four-momentum](../../../../../four-momentum.md) $P^\nu=\int T^{0\nu}d^3x$ is conserved if the boundary flux vanishes. With matter [sources](../../../../../source-quantum-field-theory.md), the [electromagnetic field](../../../../../electromagnetic-field.md) alone instead obeys $\partial_\mu T^{\mu\nu}=-F^{\nu\lambda}J_\lambda$: [energy](../../../../../energy-split.md) and momentum transfer to matter restore conservation of the total [stress-energy tensor](../../../../../stress-energy-tensor-split.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
