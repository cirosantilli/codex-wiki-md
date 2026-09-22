# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper19.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the curvature sign convention implicit in part (c): the [Jacobi field](../../../general-relativity.md#jacobi-field) equation is $D_t^2J+K_{\dot\gamma}J=0$, so the operator in a positively curved normal direction has positive [eigenvalue](../../../linear-operator-theory.md#eigenvalue). With the alternative convention $R_{\mathrm{std}}(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ used for the catalog's [Jacobi curvature operator](../../../general-relativity.md#jacobi-curvature-operator), the paper's tensor is $R=-R_{\mathrm{std}}$, and its operator is $K_v(x)=R_{\mathrm{std}}(x,v)v$. This fixes the sign throughout Q1.

Let $r(A,B,C,D)=\langle R(A,B)C,D\rangle$. Pair interchange for the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) gives

$$
\langle K_vx,y\rangle=r(v,x,v,y)=r(v,y,v,x)=\langle x,K_vy\rangle.
$$

Thus **$K_v$ is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator)** with respect to the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). The curvature sign does not affect this conclusion. The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) therefore supplies the real orthonormal [eigenbasis](../../../linear-operator-theory.md#eigenbasis) used in part (b). Also $K_vv=0$, so the tangent direction is a zero-eigenvalue direction.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $D_t=\nabla_{\dot\gamma}$ and let $P_t:T_pM\to T_{\gamma(t)}M$ denote [parallel transport](../../../fiber-bundle.md#parallel-transport). Since $\gamma$ is a [geodesic](../../../riemannian-geometry.md#geodesic), $D_t\dot\gamma=0$, while the transported vectors satisfy $D_te_i(t)=0$. The [locally symmetric Riemannian manifold](../../../riemannian-geometry.md#locally-symmetric-riemannian-manifold) condition is $\nabla R=0$. Hence the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) product rule yields

$$
D_t\bigl(R(\dot\gamma,e_i(t))\dot\gamma\bigr)
=(\nabla_{\dot\gamma}R)(\dot\gamma,e_i(t))\dot\gamma
+R(D_t\dot\gamma,e_i(t))\dot\gamma
+R(\dot\gamma,D_te_i(t))\dot\gamma
+R(\dot\gamma,e_i(t))D_t\dot\gamma=0.
$$

Both this vector field and $\lambda_i e_i(t)$ are parallel and agree at zero. Uniqueness of [parallel transport](../../../fiber-bundle.md#parallel-transport) therefore proves

$$
\boxed{K_{\dot\gamma(t)}e_i(t)=\lambda_i e_i(t),\qquad K_{\dot\gamma(t)}=P_tK_vP_t^{-1}.}
$$

The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are independent of $t$. The original PDF has $K_{\dot\gamma(t)}$ here; the converted TeX omits the dot, which would incorrectly put a point rather than a tangent vector in the operator's subscript.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Expand a [Jacobi field](../../../general-relativity.md#jacobi-field) in the parallel orthonormal [eigenbasis](../../../linear-operator-theory.md#eigenbasis): $J(t)=\sum_i j_i(t)e_i(t)$. Part (b) reduces its equation to the scalar equations $j_i''+\lambda_i j_i=0$. Define

$$
S_\lambda(t)=\begin{cases}
\sin(\sqrt\lambda\,t)/\sqrt\lambda,&\lambda>0,\\
t,&\lambda=0,\\
\sinh(\sqrt{-\lambda}\,t)/\sqrt{-\lambda},&\lambda<0,
\end{cases}
\qquad C_\lambda(t)=S_\lambda'(t).
$$

For arbitrary initial values $J(0)=\sum_i a_ie_i$ and $D_tJ(0)=\sum_i b_ie_i$, the complete solution is

$$
J(t)=\sum_i\bigl(a_iC_{\lambda_i}(t)+b_iS_{\lambda_i}(t)\bigr)e_i(t).
$$

A point at parameter $T>0$ is a [conjugate point](../../../calculus-of-variations.md#conjugate-point) of $p$ precisely when a nonzero [Jacobi field](../../../general-relativity.md#jacobi-field) vanishes at both $0$ and $T$. The first condition makes every $a_i=0$. The second requires $b_iS_{\lambda_i}(T)=0$ for every $i$, with at least one nonzero $b_i$. For $T>0$, the factors for zero and negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) never vanish; positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) give exactly the sine zeros. Therefore

$$
\boxed{T=\frac{k\pi}{\sqrt{\lambda_i}},\qquad k\in\mathbb N_{>0},\quad\lambda_i>0.}
$$

The corresponding points are $\gamma(T)$. If several positive eigenspaces have a zero at the same parameter, the conjugate multiplicity is the sum of their dimensions. This also shows that a [locally symmetric Riemannian manifold](../../../riemannian-geometry.md#locally-symmetric-riemannian-manifold) has no [conjugate points](../../../riemannian-geometry.md#conjugate-points) along a given [geodesic](../../../riemannian-geometry.md#geodesic) when that [geodesic](../../../riemannian-geometry.md#geodesic)'s [Jacobi curvature operator](../../../general-relativity.md#jacobi-curvature-operator) has no positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [connected](../../../geometry-and-topology.md#connected-space) [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) is complete when its [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) is a complete [metric space](../../../topological-analysis.md#metric-space), meaning that every [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converges in the manifold. The [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) says that for a [connected](../../../geometry-and-topology.md#connected-space) finite-dimensional [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), this is equivalent to [geodesic completeness](../../../riemannian-geometry.md#geodesic-completeness), and also to [compactness](../../../topology.md#compact-space) of every closed bounded subset. Under these equivalent conditions any two points are joined by a [minimizing geodesic](../../../riemannian-geometry.md#minimizing-geodesic), and the [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) at every point is defined on its entire [tangent space](../../../differential-geometry.md#tangent-space).

We use the usual connected, boundaryless-manifold convention for the global statements in Q2–Q5. Connectedness is essential, including for the diameter and group-growth conclusions. Without connectedness, the completeness and covering assertions apply to the target components met by the map; an unrelated incomplete component cannot be controlled by a [local isometry](../../../differential-geometry.md#local-isometry) into another component.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A [local isometry](../../../differential-geometry.md#local-isometry) preserves the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and hence [geodesics](../../../riemannian-geometry.md#geodesic), as well as the lengths of lifted curves. We first show that a complete source permits finite-length paths to lift all the way to their endpoints. Begin lifting a piecewise smooth path $c:[0,1]\to N$ from any chosen point above $c(0)$, using local inverse maps. If its lift is defined only up to a maximal $b\leq1$, then

$$
d_M(\widetilde c(s),\widetilde c(t))\leq\operatorname{length}(c|_{[s,t]})\longrightarrow0
\quad\text{as }s,t\uparrow b.
$$

Completeness gives a limit point in $M$. A local inverse at that point continues the lift, including its endpoint. Thus such a finite obstruction is impossible. Connectedness of $N$ and piecewise smooth paths from $f(p)$ to any target point prove that $f$ is onto; no prior completeness of $N$ is used in this step.

Now lift the initial position and velocity of any [geodesic](../../../riemannian-geometry.md#geodesic) in $N$. The resulting [geodesic](../../../riemannian-geometry.md#geodesic) in $M$ exists for all real time by [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem). Its image extends the original target [geodesic](../../../riemannian-geometry.md#geodesic) by uniqueness of the [geodesic](../../../riemannian-geometry.md#geodesic) initial-value problem. Hence $N$ is geodesically complete, and therefore complete.

**The converse is false for a general local [isometry](../../../riemannian-geometry.md#isometry)**, even an onto one. Give the interval $(0,4\pi)$ its ordinary metric and map it to the unit circle by $t\mapsto e^{it}$. This is an onto [local isometry](../../../differential-geometry.md#local-isometry) to a complete circle, but the sequence $t_j=1/j$ is Cauchy in the interval and has no limit there. It is not a [covering map](../../../algebraic-topology.md#covering-space): the identity point of the circle has only one preimage, whereas nearby points have two.

**The converse holds for a Riemannian covering.** If $f$ is also a [covering map](../../../algebraic-topology.md#covering-space) and $N$ is complete, every target [geodesic](../../../riemannian-geometry.md#geodesic) defined on $\mathbb R$ lifts globally with any specified initial point. A [local isometry](../../../differential-geometry.md#local-isometry) makes that lift a [geodesic](../../../riemannian-geometry.md#geodesic). Its initial velocity can be any prescribed source velocity because $df$ is an isomorphism. Thus all source [geodesics](../../../riemannian-geometry.md#geodesic) extend for all time, and $M$ is complete by the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Surjectivity was proved in part (b). Fix $q\in N$ and choose a normal ball $B=B_N(q,\varepsilon)$ on which $\exp_q$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) from the tangent ball. For each $p\in f^{-1}(q)$ define a section

$$
s_p(\exp_qv)=\exp_p\bigl((df_p)^{-1}v\bigr),\qquad |v|<\varepsilon.
$$

Completeness of $M$ guarantees that the source [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) is defined. Preservation of [geodesics](../../../riemannian-geometry.md#geodesic) and uniqueness of their initial-value problem give $f\circ s_p=\mathrm{id}_B$. Since $df$ is invertible, differentiation of this identity shows that $s_p$ is a local [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism); it is injective because it is a section. Its image $U_p$ is open, and $f:U_p\to B$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism).

These images are disjoint. If $s_p(y)=s_{p'}(y)$, lift the unique radial [geodesic](../../../riemannian-geometry.md#geodesic) from $y$ back to $q$ starting at that common point. Both section constructions give this same lift, and uniqueness forces its endpoint to be both $p$ and $p'$. Conversely, for any $x\in f^{-1}(B)$, lift that reversed radial [geodesic](../../../riemannian-geometry.md#geodesic) from $f(x)$ to $q$ starting at $x$. Completeness supplies its full finite interval; its endpoint is some $p\in f^{-1}(q)$. Reversing the lift shows $x=s_p(f(x))$. Consequently

$$
\boxed{f^{-1}(B)=\coprod_{p\in f^{-1}(q)}U_p,\qquad f|_{U_p}:U_p\longrightarrow B\text{ is a diffeomorphism}.}
$$

Every point has such an evenly covered neighborhood, proving that **the complete local [isometry](../../../riemannian-geometry.md#isometry) is a covering**. This argument does not assume a uniform positive source injectivity radius.

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [connected](../../../geometry-and-topology.md#connected-space) complete [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) is [disconnected at infinity](../../../riemannian-geometry.md#disconnected-at-infinity) when the complement of some [compact](../../../topology.md#compact-space) set has at least two unbounded [connected](../../../geometry-and-topology.md#connected-space) components. Equivalently it has at least two ends. A [line in a Riemannian manifold](../../../riemannian-geometry.md#line-in-a-riemannian-manifold) is a unit-speed [geodesic](../../../riemannian-geometry.md#geodesic) $\ell:\mathbb R\to M$ satisfying $d(\ell(s),\ell(t))=|s-t|$ for every $s,t$.

Let $K$ be the [compact](../../../topology.md#compact-space) separating set, enlarged inside a fixed [compact](../../../topology.md#compact-space) metric ball if needed for bounds. Choose $x_j,y_j$ in two different unbounded components of $M\setminus K$, with both distances from $K$ tending to infinity. By the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem), join them by unit-speed [minimizing geodesics](../../../riemannian-geometry.md#minimizing-geodesic). Every such segment meets $K$, since a path avoiding it cannot join its different components. Reparametrize a segment so that one crossing point is at time zero. Its parameter interval is $[-a_j,b_j]$, where $a_j,b_j\to\infty$ by the distances from the endpoints to $K$.

The [unit tangent bundle](../../../fiber-bundle.md#unit-tangent-bundle) over $K$ is [compact](../../../topology.md#compact-space), so a subsequence of the initial position/velocity pairs converges. Continuous dependence of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) on its initial data, and completeness, give a limiting [geodesic](../../../riemannian-geometry.md#geodesic) defined on all of $\mathbb R$. For any fixed $s<t$, the approximating segments are defined on $[s,t]$ for large $j$ and satisfy $d(\gamma_j(s),\gamma_j(t))=t-s$. Continuity of the distance passes this equality to the limit. Thus **the limiting [geodesic](../../../riemannian-geometry.md#geodesic) is a line**, proving [a line from disconnection at infinity](../../../riemannian-geometry.md#a-line-from-disconnection-at-infinity).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Cheeger-Gromoll splitting theorem](../../../second-fundamental-form.md#cheeger-gromoll-splitting-theorem) states that a complete [connected](../../../geometry-and-topology.md#connected-space) [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) with nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) that contains a [line in a Riemannian manifold](../../../riemannian-geometry.md#line-in-a-riemannian-manifold) is isometric to a [Riemannian product](../../../riemannian-geometry.md#riemannian-product) $N\times\mathbb R$ with the Euclidean metric on the line. The factor $N$ is complete and has nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature). Under the [isometry](../../../riemannian-geometry.md#isometry) one can take the given line to $\{q\}\times\mathbb R$, up to translation and reversal. A line means global minimization between every pair of its points, not merely a complete [geodesic](../../../riemannian-geometry.md#geodesic).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Suppose, for a contradiction, that $X=M\times\mathbb R$ has a complete metric with zero [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature). Since $M$ is closed and [connected](../../../geometry-and-topology.md#connected-space), the complement of $M\times[-A,A]$ has two unbounded components in any complete metric on $X$: their closures are noncompact, while closed bounded sets are [compact](../../../topology.md#compact-space) by the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem). Thus $X$ is [disconnected at infinity](../../../riemannian-geometry.md#disconnected-at-infinity), and part (a) supplies a line. The [Cheeger-Gromoll splitting theorem](../../../second-fundamental-form.md#cheeger-gromoll-splitting-theorem) gives an [isometry](../../../riemannian-geometry.md#isometry)

$$
X\cong N^3\times\mathbb R.
$$

The [Riemannian product](../../../riemannian-geometry.md#riemannian-product) curvature formula makes $N$ complete and Ricci-flat. A three-dimensional [Ricci-flat Riemannian manifold](../../../second-fundamental-form.md#ricci-flat-riemannian-manifold) is flat: for any orthonormal triple, the three trace equations are $\operatorname{Ric}_{11}=K_{12}+K_{13}$ and their cyclic companions. Solving gives $K_{ij}=\operatorname{Ric}_{ii}+\operatorname{Ric}_{jj}-\operatorname{Scal}/2=0$. Every plane can occur in such a triple, so every [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) vanishes, and hence so does the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor).

The complete [simply connected](../../../algebraic-topology.md#simply-connected-space) [universal cover](../../../algebraic-topology.md#universal-cover) of $N$ is therefore Euclidean $\mathbb R^3$, and that of $X$ is Euclidean $\mathbb R^4$. But the topological [universal cover](../../../algebraic-topology.md#universal-cover) of $X$ is $\widetilde M\times\mathbb R$. Its [deformation retraction](../../../algebraic-topology.md#deformation-retraction) onto $\widetilde M\times\{0\}$ shows that contractibility of this cover would imply contractibility of $\widetilde M$, contrary to the hypothesis. Therefore **no complete Ricci-flat metric exists on $M\times\mathbb R$**. Notice that no product assumption was made about the hypothetical original metric.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

There is a normalization issue in the printed constant. Let $\operatorname{Ric}_{\mathrm{tr}}$ denote the trace convention in the catalog's [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature), and write $\overline{\operatorname{Ric}}=\operatorname{Ric}_{\mathrm{tr}}/(n-1)$ for [normalized Ricci curvature](../../../second-fundamental-form.md#normalized-ricci-curvature), with $n\geq2$. The claimed $\pi/\sqrt k$ bound corresponds to $\overline{\operatorname{Ric}}\geq kg$, or equivalently $\operatorname{Ric}_{\mathrm{tr}}\geq(n-1)kg$. We prove the estimate in both conventions.

Take a unit-speed [minimizing geodesic](../../../riemannian-geometry.md#minimizing-geodesic) of length $L>0$ and perpendicular parallel orthonormal fields $E_1,\ldots,E_{n-1}$. Set $V_i(t)=\sin(\pi t/L)E_i(t)$. The fields vanish at the endpoints. The allowed [second variation of geodesic energy](../../../riemannian-geometry.md#second-variation-of-geodesic-energy) makes each [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form) nonnegative. Summing them gives

$$
\begin{aligned}
0\leq\sum_i I(V_i,V_i)
&=\int_0^L\left((n-1)\frac{\pi^2}{L^2}\cos^2(\pi t/L)
-\operatorname{Ric}_{\mathrm{tr}}(\dot\gamma,\dot\gamma)\sin^2(\pi t/L)\right)dt\\
&\leq\frac{n-1}{2}\left(\frac{\pi^2}{L}-kL\right)
\end{aligned}
$$

under the normalized lower bound. Thus $L\leq\pi/\sqrt k$. Completeness and the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) supply a [minimizing geodesic](../../../riemannian-geometry.md#minimizing-geodesic) between any two points, so this bounds the diameter. A closed ball of that radius about any point contains the whole manifold and is [compact](../../../topology.md#compact-space), again by the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem).

Hence the intended [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem) conclusion is

$$
\boxed{\overline{\operatorname{Ric}}\geq kg\ \Longrightarrow\ M\text{ compact},\quad\operatorname{diam}M\leq\frac\pi{\sqrt k}.}
$$

If the printed $\operatorname{Ric}\geq k$ means trace Ricci curvature instead, the same integral has lower curvature term $kL/2$ and yields

$$
\boxed{\operatorname{Ric}_{\mathrm{tr}}\geq kg\ \Longrightarrow\ \operatorname{diam}M\leq\pi\sqrt{\frac{n-1}{k}}.}
$$

The smaller bound is false under that convention when $n>2$: the round unit $S^n$ has trace Ricci tensor $(n-1)g$ and diameter $\pi$. Taking $k=n-1$ contradicts the printed $\pi/\sqrt k$ inequality. The [compactness](../../../topology.md#compact-space) assertion remains true.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

**Pointwise positive Ricci curvature does not imply [compactness](../../../topology.md#compact-space) or a finite diameter.** The [complete positively curved paraboloid](../../../second-fundamental-form.md#complete-positively-curved-paraboloid) $z=x^2+y^2$ has induced metric

$$
g=(1+4r^2)dr^2+r^2d\theta^2
$$

and [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature)

$$
K(r)=\frac{4}{(1+4r^2)^2}>0.
$$

For example, this follows from the graph formula $K=\det D^2z/(1+|Dz|^2)^2$. The metric dominates the Euclidean plane metric, so it is complete by [upward stability of Riemannian completeness](../../../riemannian-geometry.md#upward-stability-of-riemannian-completeness). Its diameter is infinite since its distance dominates Euclidean distance. On a surface the [Ricci tensor](../../../general-relativity.md#ricci-tensor) is $Kg$, so it is strictly positive everywhere, but has no uniform positive lower bound.

**There is no positive-Ricci metric on $S^2\times S^1$.** If one existed, [compactness](../../../topology.md#compact-space) of the [unit tangent bundle](../../../fiber-bundle.md#unit-tangent-bundle) would give $\operatorname{Ric}_{\mathrm{tr}}\geq cg$ for some $c>0$. The lifted metric on the [universal cover](../../../algebraic-topology.md#universal-cover) is complete by Q2 and satisfies the same positive lower bound. Part (a) makes this cover [compact](../../../topology.md#compact-space). A covering fiber is closed and discrete and therefore finite, implying a finite [fundamental group](../../../algebraic-topology.md#fundamental-group). But

$$
\pi_1(S^2\times S^1)\cong\pi_1(S^1)\cong\mathbb Z,
$$

which is infinite. This is the [finite fundamental group from a uniform positive Ricci bound](../../../second-fundamental-form.md#finite-fundamental-group-from-a-uniform-positive-ricci-bound) obstruction; it rules out every possible metric, not just the standard product metric.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Parametrize the nonconstant [closed geodesic](../../../riemannian-geometry.md#closed-geodesic) at unit speed on $[0,L]$. Its [parallel transport](../../../fiber-bundle.md#parallel-transport) around the loop fixes the tangent $\dot\gamma(0)$. Since the manifold is orientable, it preserves orientation on the full [tangent space](../../../differential-geometry.md#tangent-space), and hence has determinant one on the normal space. This normal space has odd dimension because the manifold has even dimension.

An [odd-dimensional special orthogonal transformation has a fixed vector](../../../linear-algebra.md#odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector). Indeed, nonreal [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of a real orthogonal transformation occur in conjugate pairs with product one; the real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm1$, and determinant one makes the number of $-1$ [eigenvalues](../../../linear-operator-theory.md#eigenvalue) even. Odd dimension therefore requires a $+1$ [eigenvalue](../../../linear-operator-theory.md#eigenvalue). Transport a unit fixed normal vector around the [geodesic](../../../riemannian-geometry.md#geodesic) to obtain a periodic parallel field $V$, with $D_tV=0$ and $V\perp\dot\gamma$.

The variation $\gamma_s(t)=\exp_{\gamma(t)}(sV(t))$ is defined uniformly for small $s$, because the image of the original loop is [compact](../../../topology.md#compact-space). Periodicity gives closed curves and a [homotopy](../../../algebraic-topology.md#homotopy) through loops. With the standard positive-sectional-curvature [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form), the [second variation of geodesic energy](../../../riemannian-geometry.md#second-variation-of-geodesic-energy) is

$$
E''(0)=I(V,V)=\int_0^L\bigl(|D_tV|^2-K(\dot\gamma,V)\bigr)dt
=-\int_0^LK(\dot\gamma,V)\,dt<0.
$$

The first variation vanishes for a [closed geodesic](../../../riemannian-geometry.md#closed-geodesic), since the endpoint terms cancel. Therefore $E(\gamma_s)<E(\gamma_0)=L/2$ for sufficiently small nonzero $s$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\operatorname{length}(\gamma_s)^2\leq L\int_0^L|\dot\gamma_s|^2dt
=2LE(\gamma_s)<L^2.
$$

Thus **the [closed geodesic](../../../riemannian-geometry.md#closed-geodesic) is homotopic to a strictly shorter closed curve**. This proves the [instability of a closed geodesic in positive even-dimensional curvature](../../../riemannian-geometry.md#instability-of-a-closed-geodesic-in-positive-even-dimensional-curvature); completeness of the manifold is unnecessary for this compact-loop variation. Constant loops are excluded by the usual nonconstant meaning of a [closed geodesic](../../../riemannian-geometry.md#closed-geodesic) in this assertion.

## 5

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Choose a finite symmetric generating set $S$ for $\Gamma$, let $B_S(m)$ be its [word metric](../../../geometric-group-theory.md#word-metric) ball, and fix $p\in M$. Set $D=\max_{s\in S}d(p,sp)$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and invariance of distance imply

$$
d(p,\gamma p)\leq Dm\qquad(\gamma\in B_S(m)).
$$

The [properly discontinuous group action](../../../geometric-group-theory.md#properly-discontinuous-group-action) has a finite [point stabilizer](../../../group-theory.md#stabilizer-subgroup) $H=\Gamma_p$. It also gives uniform separation of distinct orbit points. To see this, only finitely many [group](../../../group.md) elements can send $p$ into a fixed [compact](../../../topology.md#compact-space) ball about $p$, by proper discontinuity and the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem). The positive distances among this finite list, together with the radius of the ball for all other elements, have a positive lower bound $\delta$. Thus $d(\gamma p,\gamma'p)\geq\delta$ whenever the centers differ.

Take $0<\varepsilon<\delta/2$ and write $v=\operatorname{Vol}B(p,\varepsilon)>0$. Balls of radius $\varepsilon$ about distinct orbit points are disjoint and all have volume $v$, because the action is by [isometries](../../../riemannian-geometry.md#isometry). Those corresponding to words of length at most $m$ lie in $B(p,Dm+\varepsilon)$. Each orbit point arises from at most $|H|$ [group](../../../group.md) elements in $B_S(m)$, so

$$
\frac{|B_S(m)|}{|H|}\,v\leq\operatorname{Vol}B(p,Dm+\varepsilon)
\leq\omega_n(Dm+\varepsilon)^n.
$$

The final inequality is the allowed [Bishop-Gromov inequality](../../../second-fundamental-form.md#bishop-gromov-inequality) for nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature). If the entire [group](../../../group.md) fixes $p$, proper discontinuity already makes it finite and the conclusion is immediate. Otherwise the preceding separation argument applies. Therefore

$$
\boxed{|B_S(m)|\leq\frac{|H|\omega_n}{v}(Dm+\varepsilon)^n\leq C(1+m)^n.}
$$

This is [polynomial growth of a group](../../../geometric-group-theory.md#polynomial-growth-of-a-group) of degree at most $n$, proved by [polynomial group growth from orbit packing](../../../geometric-group-theory.md#polynomial-group-growth-from-orbit-packing). Neither freeness of the action nor [compactness](../../../topology.md#compact-space) of the quotient was assumed.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Put $\theta(r)=\operatorname{Vol}B(p,r)/(\omega_nr^n)$. The [Bishop-Gromov inequality](../../../second-fundamental-form.md#bishop-gromov-inequality) says that $\theta$ is nonincreasing and at most one, while smoothness gives $\theta(r)\to1$ as $r\downarrow0$. The prescribed limit at infinity is also one. Hence $\theta(r)=1$ for every $r>0$.

Here is how equality gives the global [Euclidean rigidity of maximal asymptotic volume ratio](../../../second-fundamental-form.md#euclidean-rigidity-of-maximal-asymptotic-volume-ratio). Assume first $n\geq2$. In [geodesic polar coordinates](../../../riemannian-geometry.md#geodesic-polar-coordinates) centered at $p$, let $c(\xi)$ be the cut time along unit direction $\xi$, and $J(r,\xi)$ the positive radial volume density before that time. The comparison giving the [Bishop-Gromov inequality](../../../second-fundamental-form.md#bishop-gromov-inequality) says $J(r,\xi)\leq r^{n-1}$, and

$$
\operatorname{Vol}B(p,R)=\int_{S^{n-1}}\int_0^{\min\{R,c(\xi)\}}J(r,\xi)\,dr\,d\xi.
$$

No cut time can be finite. If $c(\xi_0)<t$, then the radial segment at time $t$ is not minimizing, so $d(p,\exp_p(t\xi_0))<t$. This strict inequality persists for nearby directions by continuity, and their cut times are also at most $t$. At any radius $R>t$, that open set of directions omits all radial volume from $t$ to $R$. Even the maximal density $r^{n-1}$ cannot then give Euclidean volume, contradicting $\theta(R)=1$. Thus $c(\xi)=\infty$ for all directions. Equality of all ball volumes and continuity now force $J(r,\xi)=r^{n-1}$ everywhere.

Let $A(r)X=\nabla_X\partial_r$ on the distance sphere. This is the negative of the outward [shape operator](../../../second-fundamental-form.md#shape-operator) in the convention $S=-\nabla\nu$. Put $h=\operatorname{tr}A=\partial_r\log J$. The traced [radial Riccati equation for distance spheres](../../../riemannian-geometry.md#radial-riccati-equation-for-distance-spheres) is

$$
h'+\operatorname{tr}(A^2)+\operatorname{Ric}_{\mathrm{tr}}(\partial_r,\partial_r)=0.
$$

Since $h=(n-1)/r$, it gives

$$
\operatorname{tr}(A^2)+\operatorname{Ric}_{\mathrm{tr}}(\partial_r,\partial_r)=\frac{n-1}{r^2}.
$$

But $\operatorname{tr}(A^2)\geq h^2/(n-1)=(n-1)/r^2$ by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), and the Ricci term is nonnegative. Equality therefore holds in both, so $A=r^{-1}I$. Writing the polar metric as $dr^2+g_r$, its evolution is $\partial_rg_r=2g_r/r$. Its small-radius Euclidean limit then gives

$$
g_r=r^2g_{S^{n-1}},\qquad g=dr^2+r^2g_{S^{n-1}}.
$$

The [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) is onto by the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem), has no conjugate points, and is injective because there is no finite cut time. Explicitly, two distinct minimizing radial [geodesics](../../../riemannian-geometry.md#geodesic) reaching the same point would, after extending one past that point, create a length-minimizing broken curve with a genuine corner; smoothing the corner shortens it. That contradicts global minimization of every radial segment. Thus $\exp_p$ is a global [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), and the displayed metric proves

$$
\boxed{(M,g)\cong(\mathbb R^n,g_{\mathrm{Euclidean}})\text{ isometrically}.}
$$

In dimension one, a [connected](../../../geometry-and-topology.md#connected-space) complete manifold without boundary is a line or a circle. The circle has limiting volume ratio zero, so the hypothesis leaves only the Euclidean line.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Take the [orientation-preserving affine group of the real line](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line), written as

$$
G=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a>0,\ b\in\mathbb R\right\},\qquad
(a,b)(a',b')=(aa',b+ab').
$$

It is a [connected](../../../geometry-and-topology.md#connected-space) [Lie group](../../../lie-theory.md#lie-group), since its underlying manifold is $(0,\infty)\times\mathbb R$. We use the permitted alternative to part (a), a direct obstruction from the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group).

If a [bi-invariant Riemannian metric](../../../lie-theory.md#bi-invariant-riemannian-metric) existed, conjugation $h\mapsto ghg^{-1}$ would be an [isometry](../../../riemannian-geometry.md#isometry), being a composition of a left and a right translation. Its differential at the identity would preserve the positive [inner product](../../../linear-algebra.md#inner-product) on the [Lie algebra](../../../lie-algebra.md). Let $T$ be the nonzero infinitesimal translation,

$$
T=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad g=\begin{pmatrix}2&0\\0&1\end{pmatrix}.
$$

Direct multiplication gives $\operatorname{Ad}_gT=gTg^{-1}=2T$. Metric invariance would then imply $\|T\|^2=\|2T\|^2=4\|T\|^2$, impossible for a nonzero vector in a positive [inner product](../../../linear-algebra.md#inner-product). Therefore **this [connected](../../../geometry-and-topology.md#connected-space) affine Lie [group](../../../group.md) has no bi-invariant [Riemannian metric](../../../differential-geometry.md#riemannian-metric)**. This is the [adjoint dilation obstruction to a bi-invariant Riemannian metric](../../../lie-theory.md#adjoint-dilation-obstruction-to-a-bi-invariant-riemannian-metric); allowing an indefinite metric would be a different question.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
