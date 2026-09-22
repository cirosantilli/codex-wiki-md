<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Riemannian distance](../../../../../riemannian-distance.md) on a connected manifold is

$$
d(p,q)=\inf_c L_g(c),\qquad L_g(c)=\int_a^b\sqrt{g(\dot c,\dot c)}\,dt,
$$

where the infimum is over piecewise smooth curves joining $p$ to $q$. A connected manifold is path connected, so this infimum is finite. The metric is positive definite and induces the manifold topology; locally this follows from comparison with the Euclidean metric in a coordinate chart.

[Geodesic completeness](../../../../../geodesic-completeness.md) means that every [geodesic](../../../../../geodesic.md) with prescribed initial point and velocity extends to all parameter values in $\mathbb R$. The [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) says that, for a connected finite-dimensional [Riemannian manifold](../../../../../riemannian-manifold.md) without boundary, this is equivalent to completeness of the distance metric and equivalent to compactness of every closed bounded set. It is also equivalent to the [exponential map](../../../../../exponential-map-riemannian-geometry.md) at one, and hence every, point being defined on the whole tangent space. Under these equivalent conditions, any two points are joined by a distance-minimizing [geodesic](../../../../../geodesic.md).

A [homogeneous Riemannian manifold](../../../../../homogeneous-riemannian-manifold.md) has an [isometry](../../../../../isometry.md) group acting transitively on its points. Fix $o\in M$. Local compactness and the local metric-topology comparison give an $r>0$ such that $\overline B(o,r)$ is compact: choose a relatively compact coordinate neighborhood of $o$, then a small closed metric ball contained in it. Homogeneity makes $\overline B(p,r)$ isometric to this fixed compact ball for every $p\in M$.

Let $(p_j)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md). Its tail lies inside $\overline B(p_N,r)$ for some $N$. Compactness gives a convergent subsequence, and the Cauchy property forces the whole sequence to converge to the same limit. Thus the distance metric is complete. Hopf-Rinow now gives **every homogeneous [Riemannian manifold](../../../../../riemannian-manifold.md) is geodesically complete**. This is the [completeness of homogeneous Riemannian manifolds](../../../../../completeness-of-homogeneous-riemannian-manifolds.md); the compact ball used here is local and does not presuppose global completeness.

A [two-point homogeneous Riemannian manifold](../../../../../two-point-homogeneous-riemannian-manifold.md) has [isometries](../../../../../isometry.md) acting transitively on ordered pairs at each fixed distance. We prove the [unit tangent transitivity characterizes two-point homogeneity](../../../../../unit-tangent-transitivity-characterizes-two-point-homogeneity.md) equivalence. First suppose two-point homogeneity holds. Applying it to pairs with identical endpoints gives ordinary homogeneity. Given $p,q$ and unit tangent vectors $u,v$, choose $a>0$ sufficiently small that $au$ and $av$ lie in [normal neighbourhoods](../../../../../normal-neighbourhood.md) at $p$ and $q$. The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) and local minimizing property give

$$
d(p,\exp_p(au))=a=d(q,\exp_q(av)).
$$

There is therefore an [isometry](../../../../../isometry.md) $f$ taking these ordered pairs to one another. [Isometries](../../../../../isometry.md) preserve the [Levi-Civita connection](../../../../../levi-civita-connection.md) and [geodesics](../../../../../geodesic.md), so

$$
f(\exp_p(au))=\exp_q(a\,df_pu)=\exp_q(av).
$$

Both vectors on the right lie in the injectivity neighborhood of $\exp_q$, because $df_p$ preserves length. It follows that $df_pu=v$. Thus [isometries](../../../../../isometry.md) act transitively on the [unit tangent bundle](../../../../../unit-tangent-bundle.md).

Conversely, suppose the stated transitivity on unit tangent vectors holds. In positive dimension it implies point homogeneity, and hence completeness by the preceding argument. Consider two ordered pairs at the same distance $a>0$. Hopf-Rinow supplies unit-speed minimizing [geodesics](../../../../../geodesic.md) $\gamma_1,\gamma_2:[0,a]\to M$ joining their respective endpoints. Choose an [isometry](../../../../../isometry.md) taking $\gamma_1(0)$ to $\gamma_2(0)$ and $\dot\gamma_1(0)$ to $\dot\gamma_2(0)$. Then $f\circ\gamma_1$ and $\gamma_2$ solve the same [geodesic](../../../../../geodesic.md) initial-value problem, so they agree throughout $[0,a]$. In particular $f$ takes both endpoints of the first pair to those of the second. For $a=0$, point homogeneity suffices. If the connected manifold has dimension zero, it is a single point and both properties are immediate. Hence **two-point homogeneity is equivalent to transitivity on unit tangent vectors**. Completeness is the step allowing the local initial-direction condition to control pairs at arbitrary distance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
