<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

With no [chemotaxis](../../../../../chemotaxis.md), the stationary [oxygen](../../../../../oxygen.md) equation is $D_c c''=k\bar n$. Symmetry and the two prescribed surface values give

$$
\boxed{c(z)=c_0+\frac{k\bar n}{2D_c}\left(z^2-\frac{d^2}{4}\right).}
$$

By [Fick's first law](../../../../../fick-s-first-law.md), the vertical [oxygen](../../../../../oxygen.md) [flux](../../../../../flux.md) is $j_c=-D_cc'=-k\bar n z$. Thus each face supplies an inward [flux](../../../../../flux.md) $k\bar n d/2$ per unit area, and **the total influx is $k\bar n d$**, equal to the integrated consumption across the layer. The profile is physically nonnegative only if $c_0\ge k\bar n d^2/(8D_c)$; otherwise the constant-consumption approximation must be modified.

For bacteria retained in the fluid, impose zero bacterial [flux](../../../../../flux.md) at the faces. The stationary bacterial equation says that $j_n=-D_n n'+\mu n c'$ is constant, hence zero. Integrating $n'/n=(\mu/D_n)c'$ gives $n(z)=n_0\exp(\mu c(z)/D_n)$, with $n_0$ fixed by the total bacterial population. Substitution into the [oxygen](../../../../../oxygen.md) equation proves

$$
\boxed{c''-\frac{kn_0}{D_c}\exp(\mu c/D_n)=0.}
$$

Zero bacterial through-flux is the boundary assumption behind this equilibrium relation.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
