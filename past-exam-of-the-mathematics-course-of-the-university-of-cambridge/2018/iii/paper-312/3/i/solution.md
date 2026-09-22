<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For one [Fourier mode](../../../../../../fourier-mode.md), put $\mu=\hat{\mathbf k}\cdot\mathbf e$. The collisionless equation becomes

$$
\dot\Theta+ik\mu\Theta=\dot\phi-ik\mu\psi.
$$

Use the unweighted [Legendre polynomial](../../../../../../legendre-polynomial.md) expansion specified in the paper: $\Theta=\sum_{j\ge0}(-i)^j\Theta_jP_j(\mu)$. The [Legendre polynomial recurrence relation](../../../../../../legendre-polynomial-recurrence-relation.md) says

$$
\mu P_j=\frac{j+1}{2j+1}P_{j+1}+\frac{j}{2j+1}P_{j-1}.
$$

The coefficient of $P_\ell$ in $ik\mu\Theta$ receives contributions from $j=\ell-1$ and $j=\ell+1$. Dividing by $(-i)^\ell$ gives respectively $-k\ell\Theta_{\ell-1}/(2\ell-1)$ and $k(\ell+1)\Theta_{\ell+1}/(2\ell+3)$. The metric sources are $\dot\phi P_0$ and $-ik\psi P_1$, the latter becoming $k\psi$ after division by $(-i)$. Hence the [neutrino Boltzmann hierarchy](../../../../../../neutrino-boltzmann-hierarchy.md) is

$$
\boxed{\dot\Theta_\ell+k\left(\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}-\frac{\ell}{2\ell-1}\Theta_{\ell-1}\right)
=\delta_{\ell0}\dot\phi+\delta_{\ell1}k\psi}.
$$

The lower-neighbour term is absent for $\ell=0$. The low moments are

$$
\dot\Theta_0+\frac{k}{3}\Theta_1=\dot\phi,\qquad
\dot\Theta_1+k\left(\frac25\Theta_2-\Theta_0\right)=k\psi,\qquad
\dot\Theta_2+k\left(\frac37\Theta_3-\frac23\Theta_1\right)=0.
$$

These coefficients depend on the expansion convention. In the convention with a $(2\ell+1)$ factor, the temperature multipoles are $\Theta_\ell/(2\ell+1)$; using those multipoles without converting them would give incorrect factors in the [scalar neutrino anisotropic stress](../../../../../../scalar-neutrino-anisotropic-stress.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
