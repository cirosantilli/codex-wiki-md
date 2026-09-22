<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The Dirichlet difference [Laplacian](../../../../../../laplacian.md) has an orthogonal sine basis with [eigenvalues](../../../../../../eigenvalue.md) $-\eta_j/h^2$, where $\eta_j=4\sin^2(j\pi/(2M))$ for $j=1,\ldots,M-1$. On a mode the [theta method](../../../../../../theta-method.md) amplification is

$$
G(s)=\frac{1-(1-a)s}{1+as},\qquad s=\mu\eta_j>0.
$$

If $a\geq1/2$, the denominator is positive and

$$
(1+as)^2-[1-(1-a)s]^2=2s+(2a-1)s^2\geq0.
$$

Thus $|G(s)|\leq1$ for every mode and every $\mu>0$. Orthogonality gives a uniform discrete [L2 norm](../../../../../../l2-norm.md) contraction, not merely individual eigenvalue estimates.

If $a<0$, a positive $s=-1/a$ makes the implicit matrix singular. If $a=0$, $G=1-s$ becomes arbitrarily large. If $0<a<1/2$, $G(s)$ tends to $-(1-a)/a$, whose magnitude is greater than one. Hence **unconditional stability holds exactly for $a\geq1/2$**.

For completeness, $a<1/2$ is contractive under $\mu\eta_{\max}\leq2/(1-2a)$; the mesh-independent sufficient restriction is $\mu\leq1/[2(1-2a)]$. This follows from the same squared-modulus difference and keeps the denominator positive even for negative $a$. At $a=1/2$, very high frequencies approach amplification $-1$, so [A-stability](../../../../../../a-stability.md) does not imply damping of rough heat data. At $a=1$ the [Backward Euler method](../../../../../../backward-euler-method.md) damps them strongly; this is the [rough-data damping distinction for the theta method](../../../../../../rough-data-damping-distinction-for-the-theta-method.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [5](../../5.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
