<h1 id="31c/solution">Solution</h1>

↑ **Parent:** [31C](../31c.md)

Use the rapidly decaying real-potential normalization $u_t-6uu_x+u_{xxx}=0$. Let $D=\partial_x$, $L=-D^2+u$ and $A=4D^3-3(uD+Du)=4D^3-6uD-3u_x$. Expanding the commutator cancels its derivative terms and gives

$$
[L,A]=6uu_x-u_{xxx},\qquad \boxed{L_t=[L,A].}
$$

Thus the [KdV equation](../../../../../korteweg-de-vries-equation.md) is the compatibility condition of the [Lax pair](../../../../../lax-pair.md) $L\psi=\lambda\psi$, $\psi_t=-A\psi$. The operator $A$ is skew-adjoint on decaying functions. Its evolution transports normalized eigenfunctions unitarily, so the spectrum of $L$ is fixed; alternatively differentiating $L\psi=\lambda\psi$ and using the two equations gives $\lambda_t\psi=0$.

At each time solve the [KdV Schrodinger spectral problem](../../../../../kdv-schrodinger-spectral-problem.md). For $\lambda=k^2>0$, use the left [Jost solution](../../../../../jost-solution.md) $f_-$, normalized as $e^{-ikx}$ at $x\to-\infty$, and write $f_-\sim a(k,t)e^{-ikx}+b(k,t)e^{ikx}$ at $+\infty$. The right reflection coefficient is $R=b/a$, and transmission is $1/a$. Because $-A$ tends to $-4D^3$ at infinity, maintaining this Jost normalization gives $f_{-,t}=-Af_-+4ik^3f_-$. Substitution of its two asymptotic waves yields $a_t=0$ and $b_t=8ik^3b$. The negative discrete eigenvalues are $-\kappa_j^2$, fixed in time. A unit-normalized bound state with right tail $c_j(t)e^{-\kappa_jx}$ obeys $c_j'=4\kappa_j^3c_j$. Consequently the [Time evolution of KdV scattering data](../../../../../time-evolution-of-kdv-scattering-data.md) is

$$
\boxed{R(k,t)=R(k,0)e^{8ik^3t},\quad\kappa_j(t)=\kappa_j(0),\quad c_j(t)=c_j(0)e^{4\kappa_j^3t}.}
$$

These signs follow from the specified right-reflection convention; reversing which infinity defines reflection reverses the continuous-data phase convention.

The [inverse scattering transform](../../../../../inverse-scattering-transform.md) now solves the nonlinear evolution in three steps. Compute $R(k,0)$, the discrete eigenvalues and the norming constants from $u(x,0)$; evolve this [KdV scattering data](../../../../../kdv-scattering-data.md) by the simple formulas above; reconstruct $u$ by the [Gelfand-Levitan-Marchenko equation](../../../../../marchenko-equation.md). Explicitly set

$$
F(s,t)=\frac1{2\pi}\int_{\mathbb R}R(k,t)e^{iks}dk+\sum_jc_j(t)^2e^{-\kappa_js}
$$

and solve, for $y\ge x$,

$$
K(x,y,t)+F(x+y,t)+\int_x^\infty K(x,z,t)F(z+y,t)dz=0.
$$

The recovered potential is $\boxed{u(x,t)=-2\,dK(x,x,t)/dx}$. Each fixed discrete eigenvalue produces a soliton component, whereas the continuous scattering data encode the dispersive part. The inverse transform, rather than a linear superposition of the potentials, accounts for their nonlinear interaction.

## ↑ Ancestors (10)

1. [31C](../31c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
