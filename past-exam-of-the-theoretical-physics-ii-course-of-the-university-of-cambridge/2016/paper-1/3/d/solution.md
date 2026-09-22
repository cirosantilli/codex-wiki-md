<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The second-order terms are

$$
[S,H_t]+\frac12[S,[S,\mathcal E]]
=[S,H_t]-\frac12[S,H_t],
$$

so

$$
\boxed{H'=\mathcal E(\Delta)+H^{(2)}+O(t^3),\qquad
H^{(2)}=\frac12[S,H_t].}
$$

Here $S$ is the first-order generator. The full second-order [commutator](../../../../../commutator.md) includes terms changing the number difference by four. To retain only fixed site occupancies, keep the products $XY$ and $YX$.

With $f=f(\Delta)$ and $f_+=f(\Delta+2)$, the mixed [commutators](../../../../../commutator.md) give

$$
[fX,Y]=fXY-f_+YX,\qquad
[-f_+Y,X]=fXY-f_+YX.
$$

Thus [occupancy-preserving second-order bosonic hopping](../../../../../occupancy-preserving-second-order-bosonic-hopping.md) gives

$$
\boxed{H^{(2)}_{\rm occ}
=t\left[f(\Delta)XY-f(\Delta+2)YX\right].}
$$

For [bosons](../../../../../boson.md), [normal ordering](../../../../../normal-ordering.md) gives

$$
XY=N_a+P,\qquad YX=N_b+P,
\qquad P=\sum_{s,s'}a_s^\dagger a_{s'}b_{s'}^\dagger b_s.
$$

Consequently an explicit form in terms of the supplied function is

$$
\boxed{H^{(2)}_{\rm occ}
=t\left[f(\Delta)N_a-f(\Delta+2)N_b
+\{f(\Delta)-f(\Delta+2)\}P\right].}
$$

The operator $P$ exchanges [spin](../../../../../spin.md) labels between sites while preserving their total occupancies. Defining dimensionless Schwinger-boson [spins](../../../../../spin.md) $\mathbf s_a=\tfrac12a_s^\dagger\boldsymbol\sigma_{ss'}a_{s'}$ and similarly for $B$,

$$
P=\frac12N_aN_b+2\mathbf s_a\cdot\mathbf s_b.
$$

No factor of $\hbar^2$ is needed for these dimensionless [spins](../../../../../spin.md); for physical [spin](../../../../../spin.md) operators $\mathbf S_a=\hbar\mathbf s_a$ it becomes $2\mathbf S_a\cdot\mathbf S_b/\hbar^2$. The [spin](../../../../../spin.md) exchange belongs in the occupancy-preserving part, whereas two hops in the same direction do not.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
