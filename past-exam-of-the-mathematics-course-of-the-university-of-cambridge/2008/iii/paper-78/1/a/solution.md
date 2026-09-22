<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $y=\dot x$. The planar [autonomous differential equation](../../../../../../autonomous-system-mathematics.md) is

$$
\dot x=y,\qquad \dot y=x^2-p-(q+x)y.
$$

Its [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) have $y=0$, $x^2=p$. There are none for $p<0$, one at $p=0$, and two $x_\pm=\pm\sqrt p$ for $p>0$. At an [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) $x_*$ the [stability matrix](../../../../../../stability-matrix.md) is

$$
J_* =\begin{pmatrix}0&1\\2x_*&-(q+x_*)\end{pmatrix},\qquad
\operatorname{tr}J_*=-(q+x_*),\quad \det J_*=-2x_*.
$$

Writing $s=\sqrt p>0$, $x_+=s$ is always a [saddle equilibrium](../../../../../../saddle-equilibrium.md). At $x_-=-s$, the determinant is $2s>0$ and the trace is $s-q$: it is attracting for $q>s$ and repelling for $q<s$.

At $p=0$ and $q\ne0$, the [eigenvalues](../../../../../../eigenvalue.md) are $0,-q$; the nonzero quadratic term and parameter unfolding give a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md). At $p>0$, the trace crosses zero at $q=s$, with [eigenvalues](../../../../../../eigenvalue.md) $\pm i\sqrt{2s}$, giving a [Hopf bifurcation](../../../../../../hopf-bifurcation.md). It is nondegenerate: around $x=-s$ the equation is $\ddot\xi+(q-s)\dot\xi+2s\xi-\xi^2+\xi\dot\xi=0$. At $q=s$, a small oscillatory expansion of leading amplitude $r$ has $\langle\xi\dot\xi^2\rangle=r^4/8+O(r^5)$, so the first nonlinear damping is positive and nonzero. For example, its second-order oscillatory expansion is $\xi=r\cos(\Omega t)+r^2/(2\Omega^2)-r^2\cos(2\Omega t)/(6\Omega^2)-r^2\sin(2\Omega t)/(6\Omega)$ with $\Omega^2=2s$. Thus the small attracting [limit cycle](../../../../../../limit-cycle.md) is on the $q<s$ side. At $(p,q)=(0,0)$ the matrix has a double zero [eigenvalue](../../../../../../eigenvalue.md) and a nontrivial Jordan block, the [Bogdanov–Takens bifurcation](../../../../../../bogdanov-takens-bifurcation.md) organizing the two curves. **The local bifurcation curves are**

$$
\boxed{p=0\quad\text{and}\quad q=\sqrt p\ (p>0).}
$$

A change between node and focus away from these curves is not itself a local bifurcation.

For the requested global exclusion, suppose $x(t)$ were periodic with period $T$. Integrate the original equation over a period. The integrals of $\ddot x$, $q\dot x$, and $x\dot x=\frac12(d/dt)x^2$ vanish. Therefore

$$
\int_0^T x(t)^2\,dt=pT.
$$

The left side is nonnegative and the right side is negative when $p<0$. This contradiction proves **there are no [periodic orbits](../../../../../../periodic-orbit.md) for $p<0$**, independently of $q$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
