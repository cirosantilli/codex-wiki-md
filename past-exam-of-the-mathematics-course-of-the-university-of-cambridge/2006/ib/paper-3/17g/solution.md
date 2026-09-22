<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

In SI [units](../../../../../unit-in-a-ring.md), the source-free [Maxwell equations](../../../../../maxwell-equations.md) in vacuum are

$$
\nabla\cdot E=0,\qquad \nabla\cdot B=0,\qquad
\nabla\times E=-\partial_tB,\qquad
\nabla\times B=\mu_0\epsilon_0\partial_tE.
$$

Use complex amplitudes with phase $e^{i(\omega t-k\cdot x)}$ and take real parts at the end. The electric divergence equation gives $k\cdot E_0=0$. Faraday's equation gives $k\times E_0=\omega B_0$, so

$$
\boxed{B(x,t)=\Re\left[\frac{k\times E_0}{\omega}e^{i(\omega t-k\cdot x)}\right].}
$$

The magnetic divergence equation follows because $k\cdot(k\times E_0)=0$. Ampere's equation becomes $k\times B_0=-\mu_0\epsilon_0\omega E_0$. Since $k\times(k\times E_0)=-|k|^2E_0$, a nonzero wave satisfies

$$
\boxed{\omega^2=c^2|k|^2,\qquad c=(\mu_0\epsilon_0)^{-1/2}.}
$$

Thus both [fields](../../../../../field.md) are transverse, mutually perpendicular for linear polarization, and obey the vacuum plane-wave dispersion relation.

For the interface let $n=e_z$ point from the minus side to the plus side and write $[E]=E_+-E_-$, similarly for $B$. Applying the integral [Maxwell equations](../../../../../maxwell-equations.md) to a thin pillbox and a thin loop gives the [electromagnetic boundary conditions](../../../../../electromagnetic-boundary-condition.md)

$$
\boxed{n\cdot[E]=\sigma/\epsilon_0,\quad n\times[E]=0,\quad
n\cdot[B]=0,\quad n\times[B]=\mu_0 j.}
$$

Here $j$ is the tangential surface current. The jump notation fixes the signs, including the direction of the normal.

For the [perfect conductor](../../../../../perfect-conductor.md), take the time-varying interior [fields](../../../../../field.md) to vanish. Choose positive $k$ with $\omega=ck$. The incident [electric field](../../../../../electric-field.md) has complex form $E_0e_xe^{i\omega t+ikz}$. To cancel its tangential value at the surface, use the reflected [field](../../../../../field.md) $-E_0e_xe^{i\omega t-ikz}$, whose wavevector points upward. The total vacuum [fields](../../../../../field.md) are therefore

$$
\begin{aligned}
E&=\Re[2iE_0e^{i\omega t}\sin(kz)]e_x,\\
B&=\Re[-(2E_0/c)e^{i\omega t}\cos(kz)]e_y.
\end{aligned}
$$

The sign of each magnetic contribution follows from $B_0=k\times E_0/\omega$. At $z=0$, the [electric field](../../../../../electric-field.md) is zero and the [magnetic field](../../../../../magnetic-field.md) is tangential. The jump conditions yield

$$
\boxed{\sigma=0,\qquad
j(t)=\frac{2}{\mu_0c}\Re(E_0e^{i\omega t})e_x.}
$$

For a real incident amplitude this is $j=(2E_0/\mu_0c)\cos(\omega t)e_x$. It supplies the reflected wave while satisfying the normal-field and tangential-electric conditions. Any independently imposed static interior [field](../../../../../field.md) is separate from this oscillatory response.

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
