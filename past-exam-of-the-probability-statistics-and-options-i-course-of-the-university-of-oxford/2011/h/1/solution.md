<h1 id="h/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [inertia tensor](../../../../inertia-tensor.md) about the centroid has entries $J_{ij}=\int_B\rho(r^2\delta_{ij}-x_ix_j)\,dV$. Reflection symmetry makes every off-diagonal entry zero. Under $x=a\xi$, $y=a\eta$, $z=c\zeta$, the ellipsoid becomes the unit ball. Its three coordinate second moments are equal, and

$$
\int_{\text{ball}}\xi^2\,dV=\frac13\int_{\text{ball}}r^2\,dV=\frac{4\pi}{15}.
$$

Using the stated mass gives $\int_B\rho x^2\,dV=Ma^2/5$, the same for $y$, and $\int_B\rho z^2\,dV=Mc^2/5$. Therefore

$$
\boxed{J^{(G)}=\frac M5\operatorname{diag}(a^2+c^2,\ a^2+c^2,\ 2a^2).}
$$

For the parallel coordinate axes based at $P=(0,0,c)$, the [parallel axis theorem](../../../../parallel-axis-theorem.md) in tensor form is $J^{(P)}=J^{(G)}+M(|d|^2I-dd^T)$, where $d=P-G$. Thus

$$
\boxed{J^{(P)}=\frac M5\operatorname{diag}(a^2+6c^2,\ a^2+6c^2,\ 2a^2).}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [H](../../h.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
