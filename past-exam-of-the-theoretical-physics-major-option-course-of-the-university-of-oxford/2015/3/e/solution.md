<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Specify the [Fourier transform](../../../../fourier-transform-split.md) before performing the [Gaussian integral](../../../../gaussian-integral.md):

$$
m_j(\mathbf q)=\int d^3x\,e^{-i\mathbf q\cdot\mathbf x}m_j(\mathbf x),\qquad
m_j(\mathbf x)=\int\frac{d^3q}{(2\pi)^3}e^{i\mathbf q\cdot\mathbf x}m_j(\mathbf q).
$$

At $u=0$ the functional is diagonal in both component and momentum, with inverse kernels $q^2+t+r$, $q^2+t-r$, and $q^2+t$. The condition $0<r<t$ makes all three positive. The [covariance](../../../../covariance.md) of a [Gaussian distribution](../../../../normal-distribution.md) with statistical weight $e^{-F/(k_BT)}$ is $k_BT$ times the inverse kernel, hence

$$
\boxed{\begin{aligned}
\langle m_1(\mathbf q)m_1(\mathbf p)\rangle&=(2\pi)^3\delta^{(3)}(\mathbf q+\mathbf p)\frac{k_BT}{q^2+t+r},\\
\langle m_2(\mathbf q)m_2(\mathbf p)\rangle&=(2\pi)^3\delta^{(3)}(\mathbf q+\mathbf p)\frac{k_BT}{q^2+t-r}.
\end{aligned}}
$$

If $F$ is already the dimensionless [free energy](../../../../thermodynamic-free-energy.md) divided by $k_BT$, the numerators are one instead. Translational invariance forces opposite momenta to pair. There is no complex conjugate on the second field, so the delta function is at $\mathbf p=-\mathbf q$, not at $\mathbf p=\mathbf q$. A correlation with $m_j(\mathbf p)^*$ would have the latter convention. Rotational symmetry in real space leaves dependence on $q^2$ alone once the momentum-conservation delta function is factored out. The [correlation lengths](../../../../correlation-length.md) are $\xi_1=(t+r)^{-1/2}$ and $\xi_2=(t-r)^{-1/2}$; the second component becomes soft as $r\uparrow t$. The skipped letter in the source is preserved: this solution is part (e), with no inferred part (d).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
