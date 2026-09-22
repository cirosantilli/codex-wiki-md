<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Solving the two factors in each equation gives **$(0,0),(3,0),(0,3),(1,1)$**. The Jacobian is

$$
Df=\begin{pmatrix}2x+2y-3&2x\\-2y&3-2x-2y\end{pmatrix}.
$$

At the three boundary equilibria its [eigenvalues](../../../../../eigenvalue.md) are $3,-3$. These equilibria are [hyperbolic fixed points](../../../../../hyperbolic-equilibrium-point.md); the [Hartman-Grobman theorem](../../../../../hartman-grobman-theorem.md) gives local topological conjugacy to their saddle [linearizations](../../../../../linearization.md). At $(1,1)$ the [matrix](../../../../../matrix.md) is $\left(\begin{smallmatrix}1&2\\-2&-1\end{smallmatrix}\right)$, with [eigenvalues](../../../../../eigenvalue.md) $\pm i\sqrt3$. The [linearization](../../../../../linearization.md) is a centre, but the hyperbolic theorem does not apply there.

The nonlinear classification follows from the actual [Hamiltonian](../../../../../hamiltonian.md)

$$
\boxed{H(x,y)=xy(x+y-3),\qquad\dot x=H_y,\quad\dot y=-H_x.}
$$

Along solutions $\dot H=H_xH_y-H_yH_x=0$. At $(1,1)$, $H=-1$ and its [Hessian](../../../../../hessian-matrix.md) is $\left(\begin{smallmatrix}2&1\\1&2\end{smallmatrix}\right)$, which is positive definite. Nearby regular level curves are closed ovals around this strict minimum. Their vector field is nonzero and tangent, so each is a [periodic orbit](../../../../../periodic-orbit.md). **The nonlinear equilibrium is a centre**.

The [separatrix](../../../../../separatrix.md) level $H=0$ consists of $x=0$, $y=0$, and $x+y=3$. Within the triangle they connect the saddles as $(3,0)\to(0,0)\to(0,3)\to(3,0)$. The interior levels $-1<H<0$ are nested clockwise [periodic orbits](../../../../../periodic-orbit.md); outside the triangle the remaining level branches are unbounded. On $y=0$, flow is left for $0<x<3$ and right for $x<0$ or $x>3$; on $x=0$, it is up for $0<y<3$ and down otherwise. These directions and the invariant levels determine the full [phase portrait](../../../../../phase-portrait.md).

<a id="7e/image-hamiltonian-level-curves-and-flow-around-the-three-saddles-and-centre"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1-phase-plane.png)

**[Figure 1](#7e/image-hamiltonian-level-curves-and-flow-around-the-three-saddles-and-centre). Hamiltonian level curves and flow around the three saddles and centre**.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
