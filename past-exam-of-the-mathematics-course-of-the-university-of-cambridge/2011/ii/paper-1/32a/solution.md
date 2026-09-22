<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

A Hamiltonian system on a $2d$-dimensional [symplectic manifold](../../../../../symplectic-manifold.md) is [Liouville integrable](../../../../../integrable-hamiltonian-system.md) when it has $d$ first integrals, including the Hamiltonian, whose differentials are independent on a dense regular region and which pairwise have zero [Poisson bracket](../../../../../poisson-bracket.md). The [Arnold-Liouville theorem](../../../../../liouville-arnold-theorem.md) states that a compact connected regular common level set is a $d$-torus; near it there are [action-angle variables](../../../../../action-angle-variables.md) $(I,\theta)$ in which the Hamiltonian depends only on $I$ and the motion is $\dot I=0$, $\dot\theta=\nabla_IH$. Without compactness, the torus conclusion needs modification.

Here $q_1$ is a [cyclic coordinate](../../../../../cyclic-coordinate.md), so $p_1=\ell$ is conserved and $\{H,p_1\}=0$. The [Hamilton equations](../../../../../hamilton-s-equations.md) are

$$
\dot q_1=\frac{p_1}{q_2^2},\quad\dot q_2=p_2,\quad\dot p_1=0,\quad\dot p_2=\frac{p_1^2}{q_2^3}-\frac{k}{q_2^2}.
$$

The differentials $dH,dp_1$ are independent away from the circular-orbit critical set, establishing integrability. Put $r=q_2$; on a fixed angular-momentum level,

$$
p_2^2=2E+\frac{2k}{r}-\frac{\ell^2}{r^2}.
$$

For a bounded noncollision orbit require $\ell\ne0$ and $-k^2/(2\ell^2)<E<0$. Its two turning radii are

$$
\boxed{\alpha=\frac{k-\sqrt{k^2+2E\ell^2}}{-2E},\qquad\beta=\frac{k+\sqrt{k^2+2E\ell^2}}{-2E}.}
$$

They are positive and $\alpha<\beta$, and $p_2^2=(-2E)(r-\alpha)(\beta-r)/r^2$. In terms of $u=1/r$ and the angular coordinate, eliminating time gives $u''+u=k/\ell^2$. Thus

$$
r=\frac{\ell^2}{k[1+e\cos(q_1-q_*)]},\qquad e^2=1+\frac{2E\ell^2}{k^2}<1.
$$

After an angular change of $2\pi$ the phase-space state returns to itself, and the elapsed time is finite because $r$ is bounded away from zero and infinity. This proves periodicity; a torus alone would only guarantee quasiperiodic motion. At $E=-k^2/(2\ell^2)$ the orbit is circular and remains periodic. For $E\geq0$ the allowed radial motion is unbounded. The collision case $\ell=0$ reaches the excluded boundary $r=0$ and is not a periodic orbit in the given phase space.

With the usual action convention $(2\pi)^{-1}\oint p\,dq$, the angular cycle gives $I_1=\ell$, and the two radial legs give

$$
\boxed{I_1=p_1,\qquad I_2=\gamma\int_\alpha^\beta\frac{\sqrt{(r-\alpha)(\beta-r)}}r\,dr,\qquad\gamma=\frac{\sqrt{-2E}}\pi.}
$$

For completeness, substitute $r=(\alpha+\beta)/2+(\beta-\alpha)\cos\theta/2$ to evaluate the integral as $\pi[(\alpha+\beta)/2-\sqrt{\alpha\beta}]$. Therefore $I_2=k/\sqrt{-2E}-|\ell|$ and $H=-k^2/[2(I_2+|I_1|)^2]$. The two frequencies have equal magnitude, consistent with the closed Kepler orbits. The circular limit has $I_2=0$ and $\alpha=\beta$.

## ↑ Ancestors (11)

1. [32A](../32a.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
