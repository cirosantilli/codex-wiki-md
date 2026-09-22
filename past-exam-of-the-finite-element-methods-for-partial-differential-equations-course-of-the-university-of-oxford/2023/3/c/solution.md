<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The finite-dimensional [vector subspace](../../../../vector-subspace.md) $V_h\subset V$ is closed, so it is a [Hilbert space](../../../../hilbert-space-split.md) with the inherited [Sobolev norm](../../../../sobolev-norm.md). The [bounded bilinear form](../../../../bounded-bilinear-form.md), [coercive bilinear form](../../../../coercive-bilinear-form.md), and bounded [linear functional](../../../../linear-functional.md) estimates from part (b) restrict to $V_h$. Applying the [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) proves

$$
\boxed{\text{There is exactly one }u_h\in V_h\text{ with }a(u_h,v_h)=\ell(v_h)\quad(v_h\in V_h).}
$$

For any $v_h\in V_h$, put $d_h=v_h-u_h\in V_h$. Expansion using symmetry of the [bilinear form](../../../../bilinear-form-split.md) gives

$$
\begin{aligned}
J(v_h)-J(u_h)
&=a(u_h,d_h)-\ell(d_h)+\frac12a(d_h,d_h)\\
&=\frac12a(d_h,d_h)\geq0.
\end{aligned}
$$

Thus $u_h$ minimizes $J$ on $V_h$, uniquely by the [coercive bilinear form](../../../../coercive-bilinear-form.md) estimate. Similarly, the continuous [weak formulation](../../../../weak-formulation.md) gives the exact identity

$$
J(u_h)-J(u)=\frac12a(u_h-u,u_h-u)\geq0.
$$

Combining the two identities proves

$$
\boxed{J(v_h)\geq J(u_h)\geq J(u)\qquad(v_h\in V_h).}
$$

More precisely, $J(v_h)-J(u_h)=\tfrac12\|v_h-u_h\|_a^2$ and $J(u_h)-J(u)=\tfrac12\|u_h-u\|_a^2$, with the [energy norm](../../../../energy-norm.md) justified next. These identities connect the energy excess directly to the squared error.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
