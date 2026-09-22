<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $\alpha>0$, so a finite nonzero critical [wavenumber](../../../../../wavenumber.md) exists. The linear growth rate of a [Fourier mode](../../../../../fourier-mode.md) is $\lambda(k)=-\alpha+\mu k^2-k^4$. Maximizing over $k$ and setting that maximum to zero gives

$$
\boxed{\mu_c=2\sqrt\alpha,\qquad k_c=\alpha^{1/4}.}
$$

Set $K=k_c^2=\sqrt\alpha$. The [resonant three-wave triad](../../../../../resonant-three-wave-triad.md) has wavevectors satisfy $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$ and $\mathbf k_i\cdot\mathbf k_j=-K/2$ for $i\ne j$. With the slow time and amplitude scaling, every growth, quadratic and cubic term first enters at order $\epsilon^3$. Projection onto each critical mode removes the nonresonant correction $\Theta_3$ by the [method of multiple scales](../../../../../method-of-multiple-scales.md) solvability condition.

The parameter displacement contributes $\mu_2K A$ to the first mode. For the quadratic term, use $\nabla\cdot(\Theta_1\nabla\Theta_1)=\tfrac12\nabla^2(\Theta_1^2)$. The resonant coefficient of $\Theta_1^2$ at $\mathbf k_1$ is $2\bar B\bar C$, so its contribution is $+\gamma K\bar B\bar C$.

For the cubic gradient term, an ordered triple of modes with wavevectors $\mathbf p,\mathbf q,\mathbf r$ summing to $\mathbf k_1$ contributes $(\mathbf p\cdot\mathbf q)(\mathbf k_1\cdot\mathbf r)$ times its amplitude product. The three self-interaction permutations yield $-3K^2|A|^2A$. The six permutations of $(\mathbf k_1,\mathbf k_2,-\mathbf k_2)$ yield $-2K^2-4(\mathbf k_1\cdot\mathbf k_2)^2=-3K^2$, and likewise for the third mode. Therefore the [hexagonal convection amplitude equations](../../../../../hexagonal-convection-amplitude-equations.md) are

$$
\boxed{\begin{aligned}A_T&=\mu_2KA+\gamma K\bar B\bar C-3K^2A(|A|^2+|B|^2+|C|^2),\\B_T&=\mu_2KB+\gamma K\bar C\bar A-3K^2B(|A|^2+|B|^2+|C|^2),\\C_T&=\mu_2KC+\gamma K\bar A\bar B-3K^2C(|A|^2+|B|^2+|C|^2).\end{aligned}}
$$

For a nonzero [convection roll](../../../../../convection-roll.md), $B=C=0$ and $|A|^2=\mu_2/(3K)$, requiring $\mu_2>0$. Choose its phase so $A=a>0$. The radial perturbation decays, but a perturbation in the two other orientations gives

$$
\partial_T\begin{pmatrix}B\\\bar C\end{pmatrix}=\begin{pmatrix}0&\gamma Ka\\\gamma Ka&0\end{pmatrix}\begin{pmatrix}B\\\bar C\end{pmatrix}.
$$

The eigenvalues are $\pm|\gamma|Ka$. Thus

$$
\boxed{\gamma\ne0\quad\Longrightarrow\quad\text{every nonzero roll is unstable}.}
$$

This is [roll instability from broken up-down symmetry](../../../../../roll-instability-from-broken-up-down-symmetry.md). A growing homogeneous amplitude perturbation already proves instability, without a sideband calculation. The source's slightly asymmetric setting means nonzero quadratic coupling. If $\gamma=0$ is allowed literally, the displayed leading equations instead have a continuous sphere of constant-total-intensity states and neutral orientation perturbations. They then establish marginality, not strict growing-mode instability; higher-order effects would decide further selection. Likewise $\alpha=0$ would invalidate the assumed finite-$k_c$ triad scaling.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [Section II](../section-ii.md)
3. [Paper 77](../../paper-77-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
