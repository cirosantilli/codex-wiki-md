# Paper 131

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20131.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20131.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
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

## 1

↑ **Parent:** [Paper 131](paper-131.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [connected](../../../geometry-and-topology.md#connected-space) [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $(M,g)$, its [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) is

$$
d_g(p,q)=\inf_\gamma L_g(\gamma),
\qquad
L_g(\gamma)=\int_a^b|\dot\gamma(t)|_g\,dt,
$$

where the [infimum](../../../real-analysis.md#infimum) is over the piecewise smooth curves from $p$ to $q$. Connectedness of a [smooth manifold](../../../differential-geometry.md#smooth-manifold) implies path connectedness, so this set of curves is nonempty.

The [Gauss lemma](../../../riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) says that the differential of $\exp_p$ preserves the radial inner product: for $v,w\in T_pM$,

$$
g_{\exp_p(v)}\bigl((d\exp_p)_v v,(d\exp_p)_v w\bigr)=g_p(v,w).
$$

Consequently radial [geodesics](../../../riemannian-geometry.md#geodesic) from $p$ are orthogonal to the images of tangent vectors to spheres centred at the origin in $T_pM$. In a sufficiently small [normal neighbourhood](../../../riemannian-geometry.md#normal-neighbourhood) of $p$, this implies

$$
d_g(p,\exp_p v)=|v|_g:
$$

every competing curve has length at least the total variation of its radial coordinate, and the radial geodesic has that length.

The axioms $d_g(p,q)\geq0$, symmetry, and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follow directly from length and concatenation. Certainly $d_g(p,p)=0$. If $q\ne p$, choose a normal ball $B_g(p,r)$ that does not contain $q$. Every curve from $p$ to $q$ first meets its boundary, and its initial part has length at least $r$ by the Gauss lemma. Hence $d_g(p,q)\geq r>0$. Thus $d_g(p,q)=0$ if and only if $p=q$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Choose

$$
0<\delta<\min\{d_g(p,q),r_p\},
$$

where $r_p$ is a normal radius at $p$. Take piecewise smooth curves $c_j$ from $p$ to $q$ such that $L_g(c_j)\to d_g(p,q)$. Each $c_j$ first leaves the normal ball $B_g(p,\delta)$ at a point $p_j$. The [Gauss lemma](../../../riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) gives $d_g(p,p_j)=\delta$. The geodesic sphere

$$
S_g(p,\delta)=\exp_p\{v\in T_pM:|v|_g=\delta\}
$$

is [compact](../../../topology.md#compact-space), because the tangent-space sphere is compact and $\exp_p$ is defined on it. After taking a [convergent subsequence](../../../real-analysis.md#convergent-subsequence), let $p_j\to p_0$.

The part of $c_j$ after $p_j$ has length at least $d_g(p_j,q)$, so continuity of the [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) gives

$$
\delta+d_g(p_0,q)
\leq\lim_{j\to\infty}L_g(c_j)
=d_g(p,q).
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives the reverse inequality. Therefore

$$
\boxed{d_g(p,p_0)=\delta,
\qquad
d_g(p,p_0)+d_g(p_0,q)=d_g(p,q).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The metric $g$ is [geodesically complete](../../../riemannian-geometry.md#geodesic-completeness) when every maximal affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) is defined on all of $\mathbb R$; equivalently, $\exp_p$ is defined on every $T_pM$ for every $p\in M$.

The [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) says that for a connected [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), the following are equivalent: geodesic completeness; completeness of the [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) $d_g$; compactness of every closed bounded subset; and the existence, between every two points, of a length-minimizing geodesic. It is enough in the exponential-map formulation that $\exp_p$ be defined on all of $T_pM$ for one point $p$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The pointwise inequality $\widehat g(X,X)\geq g(X,X)$ implies

$$
L_{\widehat g}(c)\geq L_g(c)
\quad\hbox{and hence}\quad
d_{\widehat g}(x,y)\geq d_g(x,y).
$$

Every $d_{\widehat g}$-[Cauchy sequence](../../../real-analysis.md#cauchy-sequence) $(x_j)$ is therefore $d_g$-Cauchy. Since $g$ is [geodesically complete](../../../riemannian-geometry.md#geodesic-completeness), the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) makes $(M,d_g)$ a [complete metric space](../../../topological-analysis.md#complete-metric-space), so $x_j\to x$ in $d_g$ for some $x\in M$.

On a coordinate neighbourhood with compact closure around $x$, smooth positive-definite [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) are uniformly equivalent. Thus there is $C>0$ such that

$$
\widehat g(X,X)\leq Cg(X,X)
$$

there. For all sufficiently large $j$, a short $g$-geodesic from $x$ to $x_j$ stays in this neighbourhood, and hence

$$
d_{\widehat g}(x_j,x)\leq\sqrt C\,d_g(x_j,x)\longrightarrow0.
$$

**Thus $(M,d_{\widehat g})$ is complete. Another application of Hopf-Rinow shows that $\widehat g$ is geodesically complete.**

## 2

↑ **Parent:** [Paper 131](paper-131.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\gamma:[0,\ell]\to M$ be a unit-speed [geodesic](../../../riemannian-geometry.md#geodesic), let $F(s,t)$ be a smooth variation with fixed endpoints, and let

$$
T=\dot\gamma,
\qquad
V=\left.\frac{\partial F}{\partial s}\right|_{s=0}
$$

be its [variation vector field](../../../riemannian-geometry.md#variation-vector-field). Then $V(0)=V(\ell)=0$. If $V^\perp=V-\langle V,T\rangle T$ is its component normal to $\gamma$, the [second variation of Riemannian arc length](../../../riemannian-geometry.md#second-variation-of-riemannian-arc-length) is

$$
\left.\frac{d^2}{ds^2}L(F(s,\cdot))\right|_{s=0}
=I(V^\perp,V^\perp)
=\int_0^\ell\left(
|D_tV^\perp|^2-
\langle R(V^\perp,T)T,V^\perp\rangle
\right)dt.
$$

Here $D_t=\nabla_T$ is the [covariant derivative](../../../general-relativity.md#covariant-derivative) along $\gamma$, $R$ is the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor), and $I$ is the [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form). Fixed endpoints remove the boundary term. The normal projection removes a tangential change of parametrization, which does not change length to second order.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem) states that if a complete connected $n$-dimensional [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) satisfies

$$
\operatorname{Ric}\geq(n-1)k g
$$

for some $k>0$, then

$$
\operatorname{diam}(M)\leq\frac{\pi}{\sqrt k}.
$$

In particular, $M$ is compact and has finite [fundamental group](../../../algebraic-topology.md#fundamental-group).

By the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem), points $p,q\in M$ are joined by a unit-speed length-minimizing [geodesic](../../../riemannian-geometry.md#geodesic) $\gamma:[0,\ell]\to M$. Choose a parallel orthonormal frame $E_1,\ldots,E_{n-1}$ normal to $T=\dot\gamma$ and set

$$
V_i(t)=\sin\left(\frac{\pi t}{\ell}\right)E_i(t).
$$

The endpoint-vanishing fields $V_i$ arise from fixed-endpoint variations. Since $\gamma$ minimizes length, its [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form) is nonnegative on each $V_i$. Summing the [second variation of Riemannian arc length](../../../riemannian-geometry.md#second-variation-of-riemannian-arc-length) gives

$$
0\leq\sum_{i=1}^{n-1}I(V_i,V_i)
=\int_0^\ell\left[
(n-1)\frac{\pi^2}{\ell^2}\cos^2\left(\frac{\pi t}{\ell}\right)
-\operatorname{Ric}(T,T)\sin^2\left(\frac{\pi t}{\ell}\right)
\right]dt.
$$

Using the [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) bound and integrating $\sin^2$ and $\cos^2$ yields

$$
0\leq\frac{(n-1)\ell}{2}\left(\frac{\pi^2}{\ell^2}-k\right),
$$

so $\ell\leq\pi/\sqrt k$. Taking the [supremum](../../../real-analysis.md#supremum) over $p,q$ proves the diameter bound. Hopf-Rinow now makes the closed bounded space $M$ compact. Finally, the same bound applies to the complete [universal cover](../../../algebraic-topology.md#universal-cover); a compact universal cover has finite fibres over $M$, so $\pi_1(M)$ is finite.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Give $S^2\times\mathbb R$ the [Riemannian product](../../../riemannian-geometry.md#riemannian-product) of the unit round metric and the Euclidean metric. It is complete and has infinite [diameter](../../../topological-analysis.md#diameter). The round sphere has [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) $2$, while the line has scalar curvature $0$; scalar curvature is additive under Riemannian products, so

$$
\operatorname{Scal}_{S^2\times\mathbb R}=2.
$$

Thus this manifold has a strictly positive uniform lower bound on scalar curvature but violates the conclusion of the [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem). Its [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) vanishes in the $\mathbb R$ direction, showing precisely why a scalar-curvature bound is insufficient.

## 3

↑ **Parent:** [Paper 131](paper-131.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) selects the positive ordered bases in each tangent space. On an oriented $n$-dimensional [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) $\omega_g$ is the unique smooth $n$-form satisfying

$$
\omega_g(e_1,\ldots,e_n)=1
$$

for every positively oriented orthonormal frame. In positively oriented local coordinates,

$$
\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

The metric induces an [inner product](../../../linear-algebra.md#inner-product) on the bundle $\Lambda^pT^*M$ of $p$-forms. The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is the unique linear map

$$
*:\Omega^p(M)\longrightarrow\Omega^{n-p}(M)
$$

such that

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle_g\,\omega_g
$$

for all $p$-forms $\alpha,\beta$. With the [codifferential](../../../differential-form.md#codifferential) $\delta$, the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) on differential forms is

$$
\Delta=d\delta+\delta d.
$$

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) says that on a compact oriented Riemannian manifold,

$$
\Omega^p(M)
=\mathcal H^p(M)\mathbin\oplus d\Omega^{p-1}(M)
\mathbin\oplus\delta\Omega^{p+1}(M),
$$

an $L^2$-orthogonal direct sum, where $\mathcal H^p(M)=\ker\Delta$ is the finite-dimensional space of [harmonic $p$-forms](../../../differential-form.md#harmonic-differential-form). Every [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class has exactly one harmonic representative.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

**Yes to both questions.** Since $\omega_g$ has top degree, $d\omega_g=0$. Moreover $*\omega_g=1$, so the formula for the [codifferential](../../../differential-form.md#codifferential) gives

$$
\delta\omega_g=\pm *d*\omega_g=\pm *d1=0.
$$

Therefore

$$
\Delta\omega_g=(d\delta+\delta d)\omega_g=0,
$$

and the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) is a [harmonic differential form](../../../differential-form.md#harmonic-differential-form).

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) preserves both the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) and its chosen [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). At any point, extend a positively oriented orthonormal basis to a local frame whose covariant derivatives vanish at that point. Differentiating $\omega_g(e_1,\ldots,e_n)=1$ there gives $\nabla\omega_g=0$. Hence $\omega_g$ is a [parallel differential form](../../../differential-geometry.md#parallel-differential-form).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

On $p$-forms in dimension $n$, the defining identity for the [Hodge star operator](../../../differential-form.md#hodge-star-operator) gives

$$
*^2=(-1)^{p(n-p)}.
$$

For $n=4$ and $p=2$, therefore, $*^2=1$. For every $\alpha\in\Omega^2(N)$ define

$$
\alpha_+=\frac12(\alpha+*\alpha),
\qquad
\alpha_-=\frac12(\alpha-*\alpha).
$$

Then $*\alpha_+=\alpha_+$, $*\alpha_-=-\alpha_-$, and $\alpha=\alpha_++\alpha_-$. The two eigenspaces of the involution $*$ have zero intersection, which proves uniqueness. They are respectively the spaces of [self-dual](../../../differential-form.md#self-dual-differential-form) and [anti-self-dual](../../../differential-form.md#anti-self-dual-differential-form) two-forms.

Now suppose $N$ is compact and let $\beta$ be an [exact](../../../differential-form.md#exact-differential-form) three-form, say $\beta=d\theta$. Apply the [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) to the two-form $\theta$:

$$
\theta=h+d\varphi+\delta\psi.
$$

Set $a=\delta\psi$. Then $da=d\theta=\beta$ and $\delta a=\delta^2\psi=0$. For a two-form in dimension four, $\delta=-*d*$, so $d*a=0$. The self-dual form

$$
\eta=a+*a
$$

satisfies

$$
*\eta=*a+*^2a=\eta,
\qquad
d\eta=da+d*a=\beta.
$$

**Thus every exact three-form is the [exterior derivative](../../../differential-form.md#exterior-derivative) of a self-dual two-form.**

## 4

↑ **Parent:** [Paper 131](paper-131.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [line in a Riemannian manifold](../../../riemannian-geometry.md#line-in-a-riemannian-manifold) is a unit-speed [geodesic](../../../riemannian-geometry.md#geodesic) $\gamma:\mathbb R\to M$ that minimizes globally:

$$
d_g(\gamma(s),\gamma(t))=|s-t|
$$

for all $s,t\in\mathbb R$. A connected noncompact manifold is [disconnected at infinity](../../../riemannian-geometry.md#disconnected-at-infinity) if some compact set $K$ has a complement with at least two unbounded connected components.

Choose points $p_j$ and $q_j$ in two such components with

$$
d_g(p_j,K)\to\infty,
\qquad
d_g(q_j,K)\to\infty.
$$

The [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) supplies a length-minimizing geodesic $\gamma_j$ from $p_j$ to $q_j$. Its image must meet $K$, since otherwise it would connect the two different components of $M\setminus K$. Reparametrize so that $\gamma_j(0)=x_j\in K$. After taking a subsequence, compactness gives $x_j\to x\in K$ and the unit tangent vectors $\dot\gamma_j(0)$ converge to some unit $v\in T_xM$.

Both endpoint parameters tend to infinity because their distances from $K$ do. Smooth dependence of geodesics on initial data therefore makes $\gamma_j$ converge on every compact parameter interval to the complete geodesic

$$
\gamma(t)=\exp_x(tv).
$$

Every finite segment of every $\gamma_j$ minimizes length. Passing to the limit gives $d_g(\gamma(s),\gamma(t))=|s-t|$, so $\gamma$ is a line.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Cheeger-Gromoll splitting theorem](../../../second-fundamental-form.md#cheeger-gromoll-splitting-theorem) states that a complete connected [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) with nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) that contains a [line in a Riemannian manifold](../../../riemannian-geometry.md#line-in-a-riemannian-manifold) is isometric to a [Riemannian product](../../../riemannian-geometry.md#riemannian-product)

$$
N\times\mathbb R.
$$

The [Hadamard-Cartan theorem](../../../second-fundamental-form.md#cartan-hadamard-theorem) states that if a complete simply connected Riemannian manifold has nonpositive [sectional curvature](../../../second-fundamental-form.md#sectional-curvature), then for every point $p$ its [exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry)

$$
\exp_p:T_pM\longrightarrow M
$$

is a diffeomorphism. In particular, the manifold is diffeomorphic to Euclidean space and is [contractible](../../../algebraic-topology.md#contractible-space).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Suppose for a contradiction that $Y\times\mathbb R$ carries a complete [Ricci-flat metric](../../../second-fundamental-form.md#ricci-flat-riemannian-manifold). Since $Y$ is closed, the two subsets $Y\times(A,\infty)$ and $Y\times(-\infty,-A)$ are different unbounded components outside the compact set $Y\times[-A,A]$. Thus $Y\times\mathbb R$ is [disconnected at infinity](../../../riemannian-geometry.md#disconnected-at-infinity) and, by part (a), contains a [line in a Riemannian manifold](../../../riemannian-geometry.md#line-in-a-riemannian-manifold).

Its [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) is zero, so the [Cheeger-Gromoll splitting theorem](../../../second-fundamental-form.md#cheeger-gromoll-splitting-theorem) gives an isometry

$$
Y\times\mathbb R\cong N^3\times\mathbb R.
$$

The product Ricci tensor shows that $N$ is a complete three-dimensional Ricci-flat manifold. By the allowed fact, $N$ is [flat](../../../second-fundamental-form.md#flat-manifold), and hence so is $Y\times\mathbb R$.

The [universal cover](../../../algebraic-topology.md#universal-cover) of a complete flat manifold is complete, simply connected, and has zero [sectional curvature](../../../second-fundamental-form.md#sectional-curvature). The [Hadamard-Cartan theorem](../../../second-fundamental-form.md#cartan-hadamard-theorem) therefore identifies it diffeomorphically with $\mathbb R^4$, so it is contractible. On the other hand, the universal cover of the product is

$$
\widetilde{Y\times\mathbb R}=\widetilde Y\times\mathbb R,
$$

which deformation retracts onto $\widetilde Y$. It is contractible only if $\widetilde Y$ is contractible, contrary to the hypothesis. Hence no such complete Ricci-flat metric exists.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
