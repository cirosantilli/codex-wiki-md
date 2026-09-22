<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

The [reciprocal lattice](../../../../../reciprocal-lattice.md) is $\Lambda^*=\{G:G\cdot\ell\in2\pi\mathbb Z\text{ for every }\ell\in\Lambda\}$. With oriented primitive-cell volume $v_c=a_1\cdot(a_2\times a_3)$, its basis is $b_1=2\pi(a_2\times a_3)/v_c$ and the cyclic variants; thus $b_i\cdot a_j=2\pi\delta_{ij}$.

The total potential is $V(x)=\sum_\ell U(x-\ell)$. Using the [Fourier transform](../../../../../fourier-transform.md) convention $\widetilde U(q)=\int e^{-iq\cdot x}U(x)d^3x$, translation gives $\widetilde V(q)=\widetilde U(q)\Delta(q)$, with

$$
\Delta(q)=\prod_{j=1}^3\sum_{n=0}^{N_j-1}e^{-in q\cdot a_j}.
$$

The given [Born approximation](../../../../../born-approximation.md) therefore supplies the amplitude $\boxed{-m\Delta(q)\widetilde U(q)/(2\pi\hbar^2)}$. A finite [geometric series](../../../../../geometric-series.md) gives, when the denominators are nonzero,

$$
\boxed{|\Delta(q)|=\prod_{j=1}^3\left|\frac{\sin(N_jq\cdot a_j/2)}{\sin(q\cdot a_j/2)}\right|.}
$$

At reciprocal-lattice vectors each phase is one, so $|\Delta|=N_1N_2N_3$, the number of atoms. For large finite crystals these narrow peaks represent coherent [Bragg scattering](../../../../../bragg-scattering.md), with peak intensity proportional to the squared number of atoms; their finite width reflects the finite crystal size.

For the specified [face-centered cubic lattice](../../../../../face-centered-cubic-lattice.md), $v_c=a^3/4$ and

$$
b_1=\frac{2\pi}a(-\hat x+\hat y+\hat z),\quad b_2=\frac{2\pi}a(\hat x-\hat y+\hat z),\quad b_3=\frac{2\pi}a(\hat x+\hat y-\hat z).
$$

The [reciprocal lattice](../../../../../reciprocal-lattice.md) have coordinates $(2\pi/a)(h,k,l)$ with $h,k,l$ all even or all odd. The two shortest nonzero length families are $G_1=2\pi\sqrt3/a$ for $(111)$ and $G_2=4\pi/a$ for $(200)$. Elastic scattering satisfies $|q|=2|k|\sin(\theta/2)$. The assumed incident magnitude exceeds $G_2/2$, so both families are kinematically accessible, and

$$
\boxed{\frac{\sin(\theta_1/2)}{\sin(\theta_2/2)}=\frac{G_1}{G_2}=\frac{\sqrt3}{2}.}
$$

This is the angular prediction for suitable crystal orientations, or for a powder containing those orientations. A fixed single-crystal orientation must additionally satisfy the vector [Elastic Bragg scattering condition](../../../../../elastic-bragg-scattering-condition.md) $2k\cdot G+|G|^2=0$; the magnitude bound alone cannot guarantee both peaks for every incident direction.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
