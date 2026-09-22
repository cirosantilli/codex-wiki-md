<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

After the first [Bell-basis measurement](../../../../bell-basis-measurement.md) and the announced correction, the shared [Werner state](../../../../werner-state.md) has visibility $v=p^2q$. Ideal [quantum teleportation](../../../../quantum-teleportation.md) through that resource is the [depolarizing channel](../../../../quantum-depolarizing-channel.md)

$$
\mathcal D_v(\rho)=v\rho+(1-v)\frac{I_2}{2}.
$$

One way to see this is to separate the singlet branch, which teleports perfectly with the appropriate known correction convention, from $I_4/4$, which has no correlations and yields $I_2/2$.

The additional [Bell-basis measurement](../../../../bell-basis-measurement.md) at Alice's station has its own independent reliable branch of probability $q$. In its random-label branch the correction averages the four [Pauli gates](../../../../pauli-gate.md), again giving $I_2/2$. Hence the actual teleported [density matrix](../../../../density-matrix-split.md) is

$$
\boxed{\rho_{\rm out}=p^2q^2\rho_{\rm in}+(1-p^2q^2)\frac{I_2}{2}.}
$$

On sifted [BB84](../../../../bb84.md) rounds, Bob measures in Alice's preparation [basis](../../../../basis.md). The preserved component gives the correct bit with certainty; the maximally mixed component gives an error with probability $1/2$. Therefore

$$
\boxed{\mathrm{QBER}=\frac{1-p^2q^2}{2}.}
$$

For $p=q=1$ it vanishes; if either parameter is zero it is $1/2$. The result presumes successful full [Bell-basis measurement](../../../../bell-basis-measurement.md) outcomes and independent stated imperfections, without extra loss, polarization drift or dark counts.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
