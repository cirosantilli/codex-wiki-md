<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

The isotropic elastic displacement equation is $\rho\ddot u=(\lambda+\mu)\nabla(\nabla\cdot u)+\mu\nabla^2u$. With $u=\nabla\phi+\nabla\times\boldsymbol\psi$, its dilational and shear potentials satisfy

$$
\boxed{\phi_{tt}=c_P^2\nabla^2\phi,\quad\boldsymbol\psi_{tt}=c_S^2\nabla^2\boldsymbol\psi,\qquad c_P^2=(\lambda+2\mu)/\rho,\quad c_S^2=\mu/\rho.}
$$

For the specified two-dimensional potential, $u_x=\phi_x+\psi_y$, $u_y=\phi_y-\psi_x$.

Choose a real wave number $k>0$ and put $\omega=kc$. Decay into $y<0$ requires the combinations

$$
\phi=Ae^{py}e^{i(kx-\omega t)},\qquad\psi=Be^{qy}e^{i(kx-\omega t)},\quad p=k\sqrt{1-c^2/c_P^2},\quad q=k\sqrt{1-c^2/c_S^2},
$$

with $0<c<c_S$. Real parts give the physical fields. Then $u_x=ikAe^{py}+qBe^{qy}$ and $u_y=pAe^{py}-ikBe^{qy}$, times the common propagating factor. The free surface requires $\sigma_{xy}=\mu(u_{x,y}+u_{y,x})=0$ and $\sigma_{yy}=\lambda\nabla\cdot u+2\mu u_{y,y}=0$. At zero these become

$$
2ikpA+(k^2+q^2)B=0,\qquad(k^2+q^2)A-2ikqB=0.
$$

A nonzero pair exists precisely when

$$
\boxed{(k^2+q^2)^2=4k^2pq,\qquad(2-s^2)^2=4\sqrt{1-s^2}\sqrt{1-\kappa s^2},\quad s=c/c_S,\ \kappa=c_S^2/c_P^2.}
$$

For such a root, one can choose $A\ne0$ and $B=-2ikpA/(k^2+q^2)$, providing the requested wave explicitly. Squaring and excluding the static zero root gives the equivalent Rayleigh [polynomial](../../../../../polynomial-split.md)

$$
s^6-8s^4+(24-16\kappa)s^2-16(1-\kappa)=0,\qquad0<s<1.
$$

The physical positive root is unique as allowed in the question. All factors of $k$ cancel in the speed equation, so **the Rayleigh surface wave is nondispersive**, with $c$ determined only by the material constants. The potentials decay exponentially over depths of order $k^{-1}$.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
