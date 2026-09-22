<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

The Euler–Lagrange equations are

$$
\ddot x+\omega\cos(\omega t)=0,\qquad \ddot y+y=0.
$$

For $\omega\ne0$ their general solution is

$$
x=c_1t+c_2+\frac{\cos(\omega t)}\omega,\qquad
y=c_3\cos t+c_4\sin t,
$$

while for $\omega=0$, $x=c_1t+c_2$.

The action has continuous translation symmetry in $x$; it is also invariant up to endpoint terms under adding homogeneous Jacobi solutions $at+b$ to $x$ and $a\cos t+b\sin t$ to $y$. For $\omega=0$ it additionally has continuous time-translation symmetry; for nonzero $\omega$ only the corresponding discrete period remains.

A complete set of four independent first [integrals](../../../../../integral.md) is

$$
C_1=\dot x+\sin(\omega t),
$$



$$
C_2=x-tC_1-\frac{\cos(\omega t)}\omega\quad(\omega\ne0),
\qquad C_2=x-t\dot x\quad(\omega=0),
$$



$$
C_3=y\cos t-\dot y\sin t,\qquad C_4=y\sin t+\dot y\cos t.
$$

In particular $(\dot y^2+y^2)/2=(C_3^2+C_4^2)/2$ is conserved; when $\omega=0$, the usual total energy is conserved as well.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
