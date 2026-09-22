<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $V_h=\mathcal U_h\times\mathcal W_h\subset V$. The [Galerkin method](../../../../galerkin-method.md) asks for $U_h=(u_h,w_h)\in V_h$ such that

$$
\boxed{\begin{aligned}
(\nabla u_h,\nabla v_h)_0-(w_h,v_h)_0&=0&& (v_h\in\mathcal U_h),\\
(u_h,z_h)_0+(\nabla w_h,\nabla z_h)_0&=(f,z_h)_0&& (z_h\in\mathcal W_h).
\end{aligned}}
$$

Since a [finite-dimensional subspace is closed](../../../../finite-dimensional-subspace-is-closed.md), $V_h$ is itself a [Hilbert space](../../../../hilbert-space-split.md). The [bounded bilinear form](../../../../bounded-bilinear-form.md) and [coercive bilinear form](../../../../coercive-bilinear-form.md) estimates in part (a) restrict to $V_h$ with the same constants. The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) therefore gives exactly one $U_h$ for every $h$.

Put $E=U-U_h=(e_u,e_w)$. Subtracting the continuous and discrete [weak formulations](../../../../weak-formulation.md) gives [Galerkin orthogonality](../../../../galerkin-orthogonality.md):

$$
b(E,T_h)=0\qquad(T_h\in V_h).
$$

For any $Y_h=(v_h,z_h)\in V_h$, the difference $Y_h-U_h$ also belongs to $V_h$, so

$$
\begin{aligned}
\|\nabla e_u\|_0^2+\|\nabla e_w\|_0^2
&=b(E,E)\\
&=b(E,U-Y_h)+b(E,Y_h-U_h)\\
&=b(E,U-Y_h)\\
&\leq\|E\|_V\|U-Y_h\|_V.
\end{aligned}
$$

The last step uses the constant-one [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) estimate from part (a). Bounding the four terms separately by a sum would obscure the precise constant requested here.

The two [minimization problems](../../../../minimization-problem.md) over $\mathcal U_h$ and $\mathcal W_h$ are independent. Each has a [best approximation](../../../../best-approximation-in-a-normed-space.md) because its [vector subspace](../../../../vector-subspace.md) is finite-dimensional. Consequently, if

$$
D_h^2=\min_{v_h\in\mathcal U_h}\|u-v_h\|_1^2+\min_{z_h\in\mathcal W_h}\|w-z_h\|_1^2,
$$

then the preceding inequality gives exactly

$$
\boxed{\|\nabla(u-u_h)\|_0^2+\|\nabla(w-w_h)\|_0^2\leq\|U-U_h\|_V D_h.}
$$

Both errors belong to the [zero-boundary Sobolev space](../../../../zero-boundary-sobolev-space.md). Applying the [Poincaré inequality](../../../../poincare-inequality.md) componentwise now yields

$$
\frac1{1+K}\|U-U_h\|_V^2\leq\|U-U_h\|_V D_h.
$$

When $U=U_h$ the desired estimate is automatic; otherwise divide by the nonzero [norm](../../../../norm.md). Thus

$$
\boxed{\left(\|u-u_h\|_1^2+\|w-w_h\|_1^2\right)^{1/2}\leq(1+K)\left(\min_{v_h\in\mathcal U_h}\|u-v_h\|_1^2+\min_{z_h\in\mathcal W_h}\|w-z_h\|_1^2\right)^{1/2}.}
$$

The constant $C=1+K$ is independent of $h$. This is the [Céa lemma](../../../../cea-s-lemma.md) estimate for this particular [skew-coupled elliptic system](../../../../skew-coupled-elliptic-system.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
