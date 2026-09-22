# Instantaneous quadrupole luminosity of a Kepler binary

↑ **Parent:** [Quadrupole formula](quadrupole-formula.md)

For a Newtonian [Kepler orbit](kepler-orbit.md), let $M=M_1+M_2$ be the total [mass](mass.md) and $\mu=M_1M_2/M$ the [reduced mass](reduced-mass.md); put $k=GM$, $\mathbf n=\mathbf r/r$, $u=\dot r$ and $\mathbf v_\perp=\dot{\mathbf r}-u\mathbf n$, with $v^2=\dot{\mathbf r}\cdot\dot{\mathbf r}$. In the convention $q_{ij}=\mu(3r_ir_j-r^2\delta_{ij})/2$, differentiating the acceleration $\ddot{\mathbf r}=-k\mathbf r/r^3$ gives

$$
\dddot q_{ij}=\frac{\mu k}{r^2}\left[u(\delta_{ij}-3n_in_j)-6(n_iv_{\perp j}+v_{\perp i}n_j)\right].
$$

The two terms have zero cross [tensor contraction](tensor-contraction.md), with squared norms $6u^2$ and $72v_\perp^2$. Therefore $\dddot q_{ij}\dddot q_{ij}=72\mu^2k^2(v^2-11u^2/12)/r^4$. Substitution into the [quadrupole formula](quadrupole-formula.md) in this convention, $L=4G\dddot q_{ij}\dddot q_{ij}/(45c^5)$, proves the luminosity. It is nonnegative since $v^2-11u^2/12=v_\perp^2+u^2/12$. The formula uses a weak gravitational field, slow motion and leading radiation order; orbital averaging gives a secular luminosity.

## ↑ Ancestors (7)

1. [Quadrupole formula](quadrupole-formula.md)
2. [Mass quadrupole moment](mass-quadrupole-moment.md)
3. [Gravitational wave](gravitational-wave.md)
4. [General relativity](general-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Circular gravitational-wave inspiral](circular-gravitational-wave-inspiral.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-56/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322/3/solution.md)
