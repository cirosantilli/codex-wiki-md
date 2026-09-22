<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\beta>0$, symmetry of the unique stationary mean-field state gives $\mu=\langle X_1\rangle=\langle X_2\rangle$ and the balance $\lambda=\beta\mu+C\mu^2$. The fraction of the molecular removal flux using the joint reaction and the [mean molecular lifetime](../../../../../../mean-molecular-lifetime.md) are consequently

$$
E=\frac{C\mu^2}{\beta\mu+C\mu^2}=\frac{C\mu}{\beta+C\mu},\qquad
\tau=\frac\mu\lambda=\frac1{\beta+C\mu}.
$$

In particular $0\le E<1$, $C\mu=E/\tau$, and $\beta=(1-E)/\tau$.

The total loss flux of species one is $v_1^-=\mu_1(\beta+C\mu_2)$, whereas its production flux $v_1^+=\lambda$ is constant. The [reaction-rate elasticities](../../../../../../reaction-rate-elasticity.md) are therefore $H_{11}=1$ and $H_{12}=C\mu_2/(\beta+C\mu_2)=E$ at the symmetric state. Species two gives $H_{22}=1$, $H_{21}=E$. All chemical jumps in either component have unit absolute size, so their [molecular-flux-weighted reaction event sizes](../../../../../../molecular-flux-weighted-reaction-event-size.md) satisfy $\langle r_1\rangle=\langle r_2\rangle=1$. With $M_{ij}=H_{ij}/\tau_i$, this proves

$$
\boxed{M=\frac1\tau\begin{pmatrix}1&E\\E&1\end{pmatrix}.}
$$

The same matrix follows from $M=-S^{-1}AS$ with $S=\mu I$ and the drift [Jacobian matrix](../../../../../../jacobian-matrix.md) in part (b); its positive eigenvalues are the restoring rates.

For the [chemical diffusion matrix](../../../../../../chemical-diffusion-matrix.md), each component receives noise from one unit birth, its own unit death, and the joint unit loss. The unnormalized diagonal noise intensity is

$$
B_{11}=B_{22}=\lambda+\beta\mu+C\mu^2=2\lambda=2\mu/\tau.
$$

Only the joint reaction changes both components in one event. Its [stoichiometric vector](../../../../../../stoichiometric-vector.md) is $(-1,-1)$, so $B_{12}=B_{21}=(-1)(-1)C\mu^2=C\mu^2$. The positive sign reflects simultaneous decreases, rather than independent death events. Divide by the product of the means to normalize:

$$
D_{11}=D_{22}=\frac{2}{\tau\mu},\qquad D_{12}=D_{21}=C=\frac{E}{\tau\mu}.
$$

Thus the [chemical diffusion matrix](../../../../../../chemical-diffusion-matrix.md) in the [normalized stationary fluctuation-dissipation relation for a reaction network](../../../../../../normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network.md) is

$$
\boxed{D=\frac1{\tau\mu}\begin{pmatrix}2&E\\E&2\end{pmatrix}.}
$$

The unequal roles of $M$ and $D$ matter: $M$ describes restoration of perturbations, while $D$ records the covariance of the immediate stochastic reaction increments.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
