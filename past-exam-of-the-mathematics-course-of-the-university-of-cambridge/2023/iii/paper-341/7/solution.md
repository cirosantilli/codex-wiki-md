<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Assume $p\in L^\infty(-1,1)$ with $p(x)\geq p_0>0$, $q\in L^\infty(-1,1)$ with $q\geq0$, and $f\in L^2(-1,1)$. The natural energy space is the [Sobolev space](../../../../../sobolev-space-split.md) $V=H_0^1(-1,1)$. Multiplying

$$
-(py')'+qy=f
$$

by $v\in V$ and using [integration by parts](../../../../../integration-by-parts.md) gives the [weak formulation](../../../../../weak-formulation.md)

$$
\boxed{a(y,v)=\ell(v)\quad(v\in V),}
$$

where

$$
a(u,v)=\int_{-1}^1(pu'v'+quv)\,dx,
\qquad
\ell(v)=\int_{-1}^1fv\,dx.
$$

The form is bounded, and the [Poincaré inequality](../../../../../poincare-inequality.md) together with $p\geq p_0$ makes it coercive:

$$
a(v,v)\geq p_0\|v'\|_{L^2}^2\geq c\|v\|_{H^1}^2.
$$

The functional $\ell$ is bounded by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) therefore gives a unique weak solution.

Define the energy

$$
J(v)=\frac12a(v,v)-\ell(v).
$$

If $y$ is the weak solution, then for every $w\in V$,

$$
J(y+w)-J(y)
=a(y,w)-\ell(w)+\frac12a(w,w)
=\frac12a(w,w)\geq0.
$$

Thus $y$ is the unique minimizer of $J$. Conversely, differentiating $J(y+tw)$ at $t=0$ recovers $a(y,w)=\ell(w)$, so the minimization and weak problems are equivalent.

The [Ritz method](../../../../../rayleigh-ritz-method.md) chooses a finite-dimensional conforming space $V_h\subset V$ and minimizes $J$ over $V_h$. Its minimizer $y_h$ satisfies

$$
a(y_h,v_h)=\ell(v_h)qquad(v_h\in V_h).
$$

For a basis $\{\phi_j\}$ this becomes $Kc=F$, with

$$
K_{ij}=\int_{-1}^1(p\phi_j'\phi_i'+q\phi_j\phi_i)\,dx,
\qquad
F_i=\int_{-1}^1f\phi_i\,dx.
$$

Coercivity makes the stiffness matrix $K$ [symmetric positive definite](../../../../../positive-definite-matrix.md), so the discrete minimizer exists and is unique.

Subtracting the continuous and discrete equations gives [Galerkin orthogonality](../../../../../galerkin-orthogonality.md),

$$
a(y-y_h,v_h)=0\qquad(v_h\in V_h).
$$

In the [energy norm](../../../../../energy-norm.md) $\|v\|_a=\sqrt{a(v,v)}$, for any $v_h\in V_h$,

$$
\begin{aligned}
\|y-y_h\|_a^2
&=a(y-y_h,y-v_h)+a(y-y_h,v_h-y_h)\\
&=a(y-y_h,y-v_h)\\
&\leq\|y-y_h\|_a\|y-v_h\|_a.
\end{aligned}
$$

After cancellation and minimization over $v_h$, this proves the sharp symmetric form of the [Céa lemma](../../../../../cea-s-lemma.md):

$$
\boxed{\|y-y_h\|_a\leq\inf_{v_h\in V_h}\|y-v_h\|_a.}
$$

For a mesh $-1=x_0<x_1<\cdots<x_N=1$, take $V_h$ to be the continuous functions that are affine on each interval and vanish at the endpoints. The interior [piecewise-linear hat functions](../../../../../piecewise-linear-hat-function.md) form a basis, and each overlaps only its two neighbours, so $K$ is symmetric tridiagonal. In the illustrative case $p=1$ and $q=0$ on a uniform mesh, its diagonal and neighbouring entries are

$$
K_{ii}=\frac2h,
\qquad
K_{i,i+1}=K_{i+1,i}=-\frac1h.
$$

If $y\in H^2(-1,1)$, its nodal interpolant $I_hy\in V_h$ satisfies $\|y-I_hy\|_{H^1}=O(h)$. The best-approximation estimate therefore gives $\|y-y_h\|_{H^1}=O(h)$, and a standard duality argument improves the $L^2$ error to $O(h^2)$ under the corresponding elliptic regularity. This completes the route from the boundary-value problem through its variational principle to a sparse, stable finite-element approximation.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
