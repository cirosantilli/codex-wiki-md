<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each row, a [Gershgorin disc](../../../../../gershgorin-disc.md) has centre $a_{jj}=-2$ and radius $r_j=\sum_{k\ne j}|a_{jk}|$. Here $r_1=r_3=1$ and $r_2=2$, so the [Gershgorin circle theorem](../../../../../gershgorin-circle-theorem.md) gives

$$
D_1=D_3=\{z:|z+2|\le1\},\qquad D_2=\{z:|z+2|\le2\}.
$$

Since $A$ is a real [symmetric matrix](../../../../../symmetric-matrix.md), its [eigenvalues](../../../../../eigenvalue.md) are real. Intersecting the union of these [Gershgorin discs](../../../../../gershgorin-disc.md) with the real axis yields

$$
\boxed{-4\le\lambda\le0.}
$$

This bound permits zero but does not assert a zero [eigenvalue](../../../../../eigenvalue.md). The fixed-end [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) exclude it: for any nonzero real [vector](../../../../../vector.md) $v=(v_1,v_2,v_3)^T$, extend by $v_0=v_4=0$ and calculate

$$
v^T(-A)v=v_1^2+(v_2-v_1)^2+(v_3-v_2)^2+v_3^2
=\sum_{j=0}^{3}(v_{j+1}-v_j)^2>0.
$$

Indeed, equality would force every adjacent value to agree with the zero endpoint. Thus $-A$ is a [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md), $A$ is a [negative-definite matrix](../../../../../negative-definite-matrix.md), and the [eigenvalues](../../../../../eigenvalue.md) satisfy **$-4\le\lambda<0$**. The same argument works for any number of interior grid points, with prefactor $c^2/h^2>0$ in the sum. The fixed string has no zero-[frequency](../../../../../frequency.md) rigid translation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
