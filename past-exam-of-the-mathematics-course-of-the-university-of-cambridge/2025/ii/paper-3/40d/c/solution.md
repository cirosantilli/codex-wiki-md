<h1 id="40d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the wave scheme, use $v_m^n=G^n e^{im\theta}$. After multiplying by $G$, the recurrence becomes

$$
G^2+(4\mu s-2\rho)G+1=0,
\qquad
s=\sin^2\left(\frac\theta2\right).
$$

Equivalently,

$$
G+G^{-1}=2(\rho-2\mu s).
$$

Because the two roots have product one, both lie on the unit circle precisely when

$$
|\rho-2\mu s|\leq1.
$$

This must hold for every $s\in[0,1]$. At $s=0$ it requires $\rho\leq1$. Since the question assumes $1\leq\rho\leq2$, stability is possible only for $\rho=1$. The condition at $s=1$ then becomes

$$
|1-2\mu|\leq1,
$$

or $0\leq\mu\leq1$. With the stipulated $\mu>0$, the [centered three-level wave scheme](../../../../../../centered-three-level-wave-scheme.md) is stable exactly when

$$
\boxed{\rho=1,\qquad 0<\mu\leq1}.
$$

For every $\rho>1$, sufficiently long-wavelength modes have a real root larger than one, whatever the value of $\mu$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40D](../../40d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
