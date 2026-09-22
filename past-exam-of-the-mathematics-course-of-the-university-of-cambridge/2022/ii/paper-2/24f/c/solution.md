<h1 id="24f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Lift $f$ to a doubly periodic meromorphic function on $\mathbb C$. Integrate it around a fundamental parallelogram whose boundary avoids all poles. Integrals over opposite edges cancel by periodicity, while the [residue theorem](../../../../../../residue-theorem.md) gives

$$
0=\frac1{2\pi i}\int_{\partial P}f(z)\,dz
=\sum_{i=1}^n\operatorname{res}_{p_i}f.
$$

Thus the principal-part map from part (b) takes values in the codimension-one hyperplane on which the sum of residue coefficients is zero. The Mittag--Leffler existence criterion on a compact Riemann surface says that prescribed principal parts occur precisely when their residues pair trivially with every holomorphic one-form. On a complex torus the holomorphic one-forms are the scalar multiples of $dz$, so the single condition is exactly the displayed residue sum. Hence the image has dimension  
$\sum_i m_i-1$, and the kernel of constants has dimension one. For $n\geq1$,

$$
\boxed{\dim_{\mathbb C}V=\sum_{i=1}^n m_i}.
$$

Equivalently, this is the genus-one case of the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) for a positive divisor.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24F](../../24f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
