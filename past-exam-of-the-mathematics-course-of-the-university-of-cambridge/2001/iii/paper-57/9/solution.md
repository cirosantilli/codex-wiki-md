<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Let $s_*$ be the unique sonic point, $f'(s_*)=0$. For a differentiable [convex function](../../../../../convex-function.md), $f'$ is nondecreasing, negative below $s_*$ and positive above it. Split the flux into the parts propagating right and left:

$$
f^+(u)=\int_{s_*}^u\max(f'(v),0)\,dv,\qquad
f^-(u)=\int_{s_*}^u\min(f'(v),0)\,dv.
$$

Thus $f(u)=f(s_*)+f^+(u)+f^-(u)$; explicitly, $f^+(u)=f(u)-f(s_*)$ for $u>s_*$ and zero below, while $f^-(u)=f(u)-f(s_*)$ for $u<s_*$ and zero above. The [Engquist-Osher flux](../../../../../engquist-osher-flux.md) takes the right-going contribution from the left state and the left-going contribution from the right state:

$$
F(a,b)=f(s_*)+f^+(a)+f^-(b).
$$

It is consistent, $F(u,u)=f(u)$. For a transonic [rarefaction wave](../../../../../rarefaction-wave.md) with $a\le s_*\le b$ it gives $f(s_*)$; reversed transonic states give $f(a)+f(b)-f(s_*)$. This is [sonic-point splitting of a convex Engquist-Osher flux](../../../../../sonic-point-splitting-of-a-convex-engquist-osher-flux.md).

On cells of width $h$ let $U_j^n$ approximate the cell average and $\lambda=\Delta t/h$. The explicit [Engquist-Osher method](../../../../../engquist-osher-method.md) is the [finite volume method](../../../../../finite-volume-method.md)

$$
U_j^{n+1}=H(U_{j-1}^n,U_j^n,U_{j+1}^n)
=U_j^n-\lambda[F(U_j^n,U_{j+1}^n)-F(U_{j-1}^n,U_j^n)].
$$

The shared interface flux makes it conservative: sums telescope for periodic data, and the same applies on the infinite grid when boundary contributions vanish. To prove stability, choose an interval $[m,M]$ containing the initial states and impose the [CFL condition](../../../../../courant-friedrichs-lewy-condition.md)

$$
\boxed{\lambda\max_{u\in[m,M]}|f'(u)|\le1.}
$$

The partial derivatives of the update are

$$
H_a=\lambda(f^+)'(a)\ge0,\qquad
H_c=-\lambda(f^-)'(c)\ge0,\qquad
H_b=1-\lambda[(f^+)'(b)-(f^-)'(b)]=1-\lambda|f'(b)|\ge0.
$$

Therefore the update is a [monotone conservative scheme](../../../../../monotone-conservative-scheme.md). Because $H(q,q,q)=q$, componentwise comparison with the constant states $m,M$ proves $m\le U_j^{n+1}\le M$. Induction gives a mesh-independent maximum bound for every time level, and ensures the same CFL speed bound remains valid.

There is also a stronger [L1 contraction of a monotone conservative scheme](../../../../../l1-contraction-of-a-monotone-conservative-scheme.md). Let $T$ denote one whole-grid update, and let $W=\min(U,V)$ and $Z=\max(U,V)$ componentwise. Monotonicity gives $TW\le TU,TV\le TZ$. Hence $|TU-TV|\le TZ-TW$ componentwise, and conservation yields

$$
h\sum_j|(TU)_j-(TV)_j|
\le h\sum_j[(TZ)_j-(TW)_j]
=h\sum_j(Z_j-W_j)=h\sum_j|U_j-V_j|.
$$

This applies to periodic grids or summable perturbations with vanishing end fluxes. Apply the same result to $U$ and its one-cell translate; translation commutes with $T$, so

$$
\operatorname{TV}(TU)=\sum_j|(TU)_{j+1}-(TU)_j|\le\sum_j|U_{j+1}-U_j|=\operatorname{TV}(U).
$$

Thus the method is a [total variation diminishing scheme](../../../../../total-variation-diminishing-scheme.md). **Under the stated CFL condition it preserves the initial range, contracts differences in discrete $L^1$, and cannot increase total variation.** These bounds give a precise nonlinear stability result, including across the sonic point.

Convexity alone does not remove the time-step restriction omitted in the question. For the [Inviscid Burgers equation](../../../../../inviscid-burgers-equation.md) $f(u)=u^2/2$, linearize about a positive constant $U$. The update becomes $v_j^{n+1}=(1-\lambda U)v_j^n+\lambda Uv_{j-1}^n$. Its alternating Fourier mode has multiplier $1-2\lambda U$, whose modulus exceeds one if $\lambda U>1$. Hence unrestricted explicit time steps are unstable even for a convex flux with one sonic point. This is [CFL necessity for explicit Engquist-Osher stability](../../../../../cfl-necessity-for-explicit-engquist-osher-stability.md).

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
