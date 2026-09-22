<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $e=u-u_h$ and $V=\{v\in H^1(0,1):v(1)=0\}$. The primal solution and its [finite element](../../../../../finite-element.md) approximation lie in the same affine space with value one at the right endpoint, so $e\in V$. Use

$$
a(w,v)=\int_0^1(pw'v'+qwv).
$$

Define the dual solution by

$$
\boxed{-(pz')'+qz=e,\qquad z'(0)=0,\quad z(1)=0.}
$$

Equivalently $z\in V$ satisfies $a(v,z)=(e,v)$ for every $v\in V$. Positivity of $p,q$ gives a unique solution, and one-dimensional regularity gives $z\in H^2$.

Then $\|e\|_{L^2}^2=a(e,z)$. The nodal interpolant $I_hz$ belongs to the homogeneous [finite element](../../../../../finite-element.md) test space, so [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) gives $a(e,I_hz)=0$. Set $w=z-I_hz$. Using the primal weak equation,

$$
\|e\|_{L^2}^2=(f,w)-a(u_h,w).
$$

Integrate the [derivative](../../../../../derivative.md) term separately on each element. Since $w$ vanishes at every [mesh](../../../../../finite-element-mesh.md) node, all endpoint flux and flux-jump terms vanish. Therefore

$$
\boxed{\|e\|_{L^2}^2
=\sum_i\int_{x_{i-1}}^{x_i}R_h(z-I_hz)\,dx.}
$$

The absence of jump terms here follows specifically from one-dimensional nodal [interpolation](../../../../../interpolation-split.md); it is not an assumption that the [finite element](../../../../../finite-element.md) flux itself is continuous.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
