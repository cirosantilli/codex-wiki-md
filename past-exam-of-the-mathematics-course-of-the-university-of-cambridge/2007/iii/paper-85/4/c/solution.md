<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The proposed transformation diagonalizes the time-circle action, but the two resulting coordinates have opposite temporal weights. Direct calculation gives

$$
\rho(z_1,z_2)=(iz_1,iz_2),\qquad
m_x(z_1,z_2)=(\bar z_2,\bar z_1),\qquad
\tau_\phi(z_1,z_2)=(e^{-i\phi}z_1,e^{i\phi}z_2).
$$

Use the [Hopf coordinates for two real representation copies](../../../../../../hopf-coordinates-for-two-real-representation-copies.md)

$$
q_1=z_1,\qquad q_2=\bar z_2,
$$

so the temporal circle is common complex phase multiplication. Writing its phase action as $T_\theta q=e^{i\theta}q$, with $\theta=-\phi$, the spatial generators become $\rho(q_1,q_2)=(iq_1,-iq_2)$ and $m_x(q_1,q_2)=(q_2,q_1)$. The combined action has kernel $K=\{(1,1),(\rho^2,-1)\}$.

Three nonconjugate [complex axial isotropy subgroups](../../../../../../complex-axial-isotropy-subgroup.md) and their fixed complex lines are

$$
\begin{aligned}
\Sigma_R&=\langle(\rho,e^{-i\pi/2})\rangle,&\operatorname{Fix}(\Sigma_R)&=\{(q,0):q\in\mathbb C\},\\
\Sigma_A&=\langle(m_x,1),(\rho^2,-1)\rangle,&\operatorname{Fix}(\Sigma_A)&=\{(q,q):q\in\mathbb C\},\\
\Sigma_D&=\langle(\rho m_x,-1),(\rho^2,-1)\rangle,&\operatorname{Fix}(\Sigma_D)&=\{(q,iq):q\in\mathbb C\}.
\end{aligned}
$$

For example $(\rho,e^{-i\pi/2})$ acts as $(q_1,-q_2)$, forcing $q_2=0$; reflection forces $q_2=q_1$; and $(\rho m_x,-1)$ acts as $(-iq_2,iq_1)$, forcing $q_2=iq_1$. Each is the full stabilizer of a generic nonzero point of that line and includes $K$. The rotational spatial projection of $\Sigma_R$ distinguishes it from the standing types; the other two use the two nonconjugate reflection-axis classes in $D_4$.

The [equivariant Hopf theorem](../../../../../../equivariant-hopf-theorem.md) guarantees the corresponding three generic primary branches. They are a [rotating-wave branch of an equivariant Hopf bifurcation](../../../../../../rotating-wave-branch-of-an-equivariant-hopf-bifurcation.md), an axial [standing-wave branch of an equivariant Hopf bifurcation](../../../../../../standing-wave-branch-of-an-equivariant-hopf-bifurcation.md), and a diagonal standing-wave branch. In the literal $z$ coordinates their fixed spaces are $z_2=0$, $z_2=\bar z_1$, and $z_2=-i\bar z_1$, respectively; using a common $e^{i\Omega t}$ in both original $z$ coordinates would not describe these standing branches correctly.

To interpret them physically, invert the transformation: $w_1=z_1+z_2$, $w_2=-i(z_1-z_2)$. For $q=Re^{i\Omega t}$, the three representatives are

$$
\boxed{\begin{aligned}
R:&\quad(w_1,w_2)=(q,-iq),\\
A:&\quad(w_1,w_2)=(2R\cos\Omega t,\ 2R\sin\Omega t),\\
D:&\quad(w_1,w_2)=R(1-i)(\cos\Omega t-\sin\Omega t,\ \cos\Omega t+\sin\Omega t).
\end{aligned}}
$$

The rotating solution changes spatial direction throughout the cycle. The standing solutions remain on a fixed spatial axis or diagonal while the two real-copy amplitudes oscillate in quadrature. Reflections exchange the two rotating chiralities; rotations generate the other representatives within each standing-wave type.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
