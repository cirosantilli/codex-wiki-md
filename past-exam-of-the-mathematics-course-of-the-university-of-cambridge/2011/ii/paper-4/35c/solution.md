<h1 id="35c/solution">Solution</h1>

↑ **Parent:** [35C](../35c.md)

For a localized charge distribution and a field point $r$ outside it, expand the Coulomb [kernel](../../../../../kernel-of-a-linear-map.md):

$$
\frac1{|r-x|}=\frac1r+\frac{r\cdot x}{r^3}+\frac{3(r\cdot x)^2-r^2|x|^2}{2r^5}+O(|x|^3/r^4).
$$

Integrating against the charge density gives the [electrostatic multipole expansion](../../../../../electric-multipole-expansion.md)

$$
\boxed{\phi(r)=\frac1{4\pi\epsilon_0}\left[\frac{Q}{r}+\frac{p_i r_i}{r^3}+\frac{Q_{ij}r_ir_j}{2r^5}+\cdots\right],}
$$

where $Q=\int\rho\,d^3x$, $p_i=\int\rho x_i\,d^3x$ is the [electric dipole moment](../../../../../electric-dipole-moment.md), and the symmetric trace-free [electric quadrupole moment](../../../../../electric-quadrupole-moment.md) is $Q_{ij}=\int\rho(3x_ix_j-|x|^2\delta_{ij})\,d^3x$. This states the tensor normalization explicitly.

For the tetrahedral point charges, the total charge is zero and the three other [vertex](../../../../../vertex-graph-theory.md) vectors sum to minus $(1,1,1)$. Hence

$$
\boxed{\mathbf p=4q(1,1,1).}
$$

Every [vertex](../../../../../vertex-graph-theory.md) has $|x|^2=3$ and each $x_i^2=1$, so each diagonal quadrupole entry vanishes. For each distinct coordinate pair the charge-weighted sum of $x_ix_j$ is $4q$, yielding

$$
\boxed{(Q_{ij})=12q\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix}.}
$$

The tensor is trace-free as required. If the alternative raw second-moment convention is used, its off-diagonal entries are $4q$ and the [kernel](../../../../../kernel-of-a-linear-map.md) contraction has the corresponding factor of three; the physical potential is unchanged.

## ↑ Ancestors (10)

1. [35C](../35c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
