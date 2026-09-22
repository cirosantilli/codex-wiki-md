<h1 id="b/7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $e_h=u-u_h$ and $w=z-I_hz$. [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) gives $a(e_h,I_hz)=0$, so the dual identity becomes

$$
\int_0^1e_h\psi=a(e_h,z)=a(e_h,w)=\int_0^1fw-a(u_h,w).
$$

On $I_i=(x_{i-1},x_i)$, $u_h'$ is constant and $w$ is zero at both endpoints. Consequently $\int_{I_i}u_h'w'=u_h'[w]_{x_{i-1}}^{x_i}=0$. Defining the element residual by

$$
\boxed{R(u_h)|_{I_i}=f-e^xu_h}
$$

gives

$$
\int_0^1(u-u_h)\psi=\sum_{i=1}^N\int_{I_i}R(u_h)(z-I_hz).
$$

No derivative-jump terms survive, because this [interpolation](../../../../../interpolation-split.md) error vanishes at every mesh node. This is the mechanism of the [explicit one-dimensional dual residual bound in L2](../../../../../explicit-one-dimensional-dual-residual-bound-in-l2.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
