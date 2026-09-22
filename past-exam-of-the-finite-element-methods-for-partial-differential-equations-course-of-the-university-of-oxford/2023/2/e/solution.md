<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $e=u-u_h\in V$. The [Aubin–Nitsche duality argument](../../../../aubin-nitsche-duality-argument.md) uses the dual [weak formulation](../../../../weak-formulation.md)

$$
z\in V,\qquad a(v,z)=(e,v)_0\quad(v\in V).
$$

By symmetry of $a$ and the [Lax-Milgram theorem](../../../../lax-milgram-theorem.md), this has a unique solution. Taking $v=z$ and using the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) shows

$$
\|z\|_1^2=(e,z)_0\leq\|e\|_0\|z\|_0\leq\|e\|_0\|z\|_1,
\qquad \|z\|_1\leq\|e\|_0.
$$

We must justify $H^2$ [elliptic regularity](../../../../elliptic-regularity.md) for this dual problem from the result actually supplied. That result concerns $\Delta$, whereas the dual equation is $-\Delta z+z=e$. Put $g=z-e\in L^2(\Omega)$. The given result produces $w\in H^2(\Omega)\cap V$ with $\Delta w=g$, zero [normal derivative](../../../../normal-derivative.md) on $\Gamma_N$, and

$$
\|w\|_{H^2(\Omega)}\leq C_3\|z-e\|_0\leq2C_3\|e\|_0.
$$

By [Green's first identity](../../../../green-s-first-identity.md), for every $v\in V$,

$$
(\nabla w,\nabla v)_0=-(g,v)_0=(e-z,v)_0=(\nabla z,\nabla v)_0.
$$

Set $v=w-z$. Then $\nabla(w-z)=0$. On the connected [triangle](../../../../triangle.md), a [Sobolev function with zero weak gradient](../../../../sobolev-function-with-zero-weak-gradient.md) is constant, and its zero [Sobolev trace](../../../../trace-operator.md) on $\Gamma_D$ forces that constant to be zero. Hence $z=w$, proving

$$
\boxed{z\in H^2(\Omega)\cap V,\qquad\|z\|_{H^2(\Omega)}\leq2C_3\|e\|_0.}
$$

This proves the needed [reaction-diffusion regularity from Laplacian regularity](../../../../reaction-diffusion-regularity-from-laplacian-regularity.md) without assuming the dual solution already has second [derivatives](../../../../derivative.md) in the [L2 space](../../../../l2-space-is-a-hilbert-space.md).

Only $H^2$ regularity is available for $z$. Use its continuous [piecewise-linear](../../../../piecewise-linear-function.md) [interpolant](../../../../interpolant.md) $L_hz$, which belongs to the quadratic [conforming finite element space](../../../../conforming-finite-element-space.md) $V_h$ because $\mathcal P_1(K)\subset\mathcal P_2(K)$. It has the same zero [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) and satisfies the [finite element interpolation estimate](../../../../finite-element-interpolation-estimate.md)

$$
\|z-L_hz\|_1\leq C_Lh\|z\|_{H^2(\Omega)}.
$$

Thus no $H^3$ assumption on the dual solution is necessary. Taking $v=e$ in the dual [weak formulation](../../../../weak-formulation.md) and using [Galerkin orthogonality](../../../../galerkin-orthogonality.md) gives

$$
\begin{aligned}
\|e\|_0^2
&=a(e,z)=a(e,z-L_hz)\\
&\leq\|e\|_1\|z-L_hz\|_1\\
&\leq2C_3C_Lh\|e\|_1\|e\|_0.
\end{aligned}
$$

If $\|e\|_0=0$, the desired bound holds. Otherwise divide by $\|e\|_0$ and use part (d):

$$
\boxed{\|u-u_h\|_{L^2(\Omega)}\leq2C_3C_Lh\|u-u_h\|_{H^1(\Omega)}\leq C_2h^3\|u\|_{H^3(\Omega)},\qquad C_2=2C_3C_LC_1.}
$$

All constants depend only on the fixed [triangle](../../../../triangle.md) and [shape regularity](../../../../shape-regular-mesh.md). The acute-angle assumption enters through the supplied mixed-boundary [elliptic regularity](../../../../elliptic-regularity.md) result.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
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
