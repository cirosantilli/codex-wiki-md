<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Integral identity and representation.** Define $L=\nabla^2+k^2$ and take $n$ to be the outward unit normal. The [product rule](../../../../product-rule.md) gives

$$
\nabla\cdot(\phi\nabla\psi-\psi\nabla\phi)=\phi\nabla^2\psi-\psi\nabla^2\phi=\phi L\psi-\psi L\phi.
$$

The $k^2\phi\psi$ terms cancel. Integrating and applying the [divergence theorem](../../../../divergence-theorem.md) proves the [Helmholtz equation](../../../../helmholtz-equation.md) version of [Green's second identity](../../../../green-second-identity.md):

$$
\boxed{\int_V(\phi L\psi-\psi L\phi)\,dV=\int_S(\phi\partial_n\psi-\psi\partial_n\phi)\,dS.}
$$

Choose the [Dirichlet Green function](../../../../dirichlet-green-function.md) with the sign convention

$$
L_xG(x,x')=\delta(x-x'),\qquad G(x,x')=0\quad(x\in S),
$$

where $\delta$ is the three-dimensional [Dirac delta](../../../../dirac-delta-function.md). Substitute $\psi=G$, use $L\phi=f$, and evaluate the [Dirac delta](../../../../dirac-delta-function.md) integral. The boundary term containing $G$ vanishes and $\phi=g$ on $S$, leaving

$$
\phi(x')-\int_VG(x,x')f(x)\,dV=\int_Sg(x)\partial_nG(x,x')\,dS.
$$

Hence

$$
\boxed{\phi(x')=\int_VG(x,x')f(x)\,dV+\int_Sg(x)\partial_nG(x,x')\,dS.}
$$

The choice of sign in the [Green function](../../../../green-s-function-split.md) equation matters: it fixes both the source normalization and these signs. For a bounded region this construction presumes that the chosen $k^2$ is not a [Dirichlet eigenvalue](../../../../dirichlet-eigenvalue.md) of $-\nabla^2$; at such an eigenvalue a Green inverse for arbitrary data does not exist.

**Infinite space.** Put $r=|x-x'|$. Away from the source, spherical symmetry reduces the [Helmholtz equation](../../../../helmholtz-equation.md) to

$$
G''+\frac2rG'+k^2G=0,\qquad (rG)''+k^2(rG)=0.
$$

For $k\ne0$ its general radial solution is

$$
G(r)=\frac{A\cos kr+B\sin kr}{r}.
$$

Integrate $LG=\delta$ over a ball of radius $\varepsilon$ about the source. The [divergence theorem](../../../../divergence-theorem.md) yields

$$
4\pi\varepsilon^2G'(\varepsilon)+k^2\int_{r<\varepsilon}G\,dV=1.
$$

Since $G=A/r+Bk+O(r)$, the volume term is $O(\varepsilon^2)$ and the flux tends to $-4\pi A$. Therefore $A=-1/(4\pi)$, while $B$ remains free:

$$
\boxed{G(r)=-\frac{\cos kr}{4\pi r}+B\frac{\sin kr}{r},\qquad r>0.}
$$

The $B$ term extends regularly through the source and solves the homogeneous [Helmholtz equation](../../../../helmholtz-equation.md), so it cannot change the unit [Dirac delta](../../../../dirac-delta-function.md) normalization. A condition at infinity is needed to select it. For example, with time dependence $e^{-i\omega t}$, the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) is $-e^{ikr}/(4\pi r)$, corresponding to $B=-i/(4\pi)$.

**Zero wavenumber.** For fixed finite $B$, $\sin(kr)/r\to0$ as $k\to0$, and

$$
\boxed{G(r)\longrightarrow-\frac1{4\pi r},\qquad\nabla^2G=\delta.}
$$

This is the decaying [Green function of the Laplacian](../../../../green-function-of-the-laplacian.md). Directly at $k=0$, the general radial solution is $A/r+C$; source normalization fixes $A=-1/(4\pi)$, and decay at infinity removes $C$. If the free parameter depends on $k$ as $B(k)\sim C/k$, the limit instead includes that arbitrary homogeneous constant. Thus the usual Laplace limit holds for a fixed parameter, or after a suitable condition at infinity has been selected.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
