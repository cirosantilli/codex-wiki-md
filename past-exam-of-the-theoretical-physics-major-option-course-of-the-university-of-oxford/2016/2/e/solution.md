<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the unitary discrete [Fourier transform](../../../../fourier-transform-split.md) $a_j=L^{-1/2}\sum_ke^{ikj}a_k$, where $k=2\pi n/L$. Then

$$
H_{\rm LSW}=\sum_k\left[\alpha_k a_k^\dagger a_k+
\frac{\beta_k}{2}(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)\right],
$$

with $\alpha_k=S[2J^x-(J^y+J^z)\cos k]$ and $\beta_k=-S(J^y-J^z)\cos k$. The factor $1/2$ accounts for the duplicated $k,-k$ pair in the full momentum sum.

Make a bosonic [Bogoliubov transformation](../../../../bogoliubov-transformation.md) $a_k=\cosh\theta_k\,b_k+\sinh\theta_k\,b_{-k}^\dagger$. Its coefficients preserve the [canonical commutation relation](../../../../canonical-commutation-relation.md) because $\cosh^2\theta_k-\sinh^2\theta_k=1$. The coefficient of the pair term vanishes when $\tanh2\theta_k=-\beta_k/\alpha_k$. Thus

$$
\boxed{H_{\rm LSW}=\sum_k\varepsilon_k b_k^\dagger b_k+\text{constant},\qquad
\varepsilon_k=2S\sqrt{(J^x-J^y\cos k)(J^x-J^z\cos k)}.}
$$

The dropped constant is $\tfrac12\sum_k(\varepsilon_k-\alpha_k)$ in addition to the classical [ground-state energy](../../../../ground-state-energy.md). Since $J^x>J^y>J^z>0$, $\alpha_k>|\beta_k|$ at every $k$, so the [bosonic Bogoliubov diagonalization](../../../../bosonic-bogoliubov-diagonalization.md) is stable. The minimum occurs at $k=0$ and gives the [energy gap](../../../../energy-gap.md) $2S\sqrt{(J^x-J^y)(J^x-J^z)}$. In the isotropic limit the pair coefficient vanishes and the familiar quadratic small-$k$ ferromagnetic [dispersion relation](../../../../dispersion-relation-split.md) is recovered.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
