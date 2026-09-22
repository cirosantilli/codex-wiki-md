<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Again assume the intended trace [Ricci curvature](../../../../../../ricci-curvature.md) bound $\operatorname{Ric}\geq(n-1)kg$, and put $D=\pi/\sqrt k$. Compactness from the [Bonnet-Myers theorem](../../../../../../myers-s-theorem.md) ensures that the diameter is attained: choose $p,q$ with $d(p,q)=D$. For $0<r<D$, the open balls $B(p,r)$ and $B(q,D-r)$ are disjoint, because a point in both would violate the [triangle inequality](../../../../../../triangle-inequality.md).

The clearly stated [Bishop volume comparison with a positive-curvature model](../../../../../../bishop-volume-comparison-with-a-positive-curvature-model.md) from part (b), applied between radius $r$ and radius $D$, gives

$$
V_p(r)\geq\frac{v_k(r)}{v_k(D)}\operatorname{Vol}M,\qquad V_q(D-r)\geq\frac{v_k(D-r)}{v_k(D)}\operatorname{Vol}M.
$$

Here both radius-$D$ ball volumes equal the total volume, as shown in part (b). The symmetry $s_k(D-t)=s_k(t)$ gives

$$
v_k(r)+v_k(D-r)=v_k(D).
$$

The two lower bounds therefore sum to $\operatorname{Vol}M$, while disjointness bounds that same sum above by $\operatorname{Vol}M$. Both inequalities must be equalities. In particular

$$
\frac{V_p(r)}{v_k(r)}=\frac{\operatorname{Vol}M}{v_k(D)}\qquad(0<r<D).
$$

Letting $r\downarrow0$, the local Euclidean volume asymptotic gives one on the left. Thus $\operatorname{Vol}M=v_k(D)$, and the detailed equality proof in part (b) applies. We obtain

$$
\boxed{\operatorname{diam}M=\pi/\sqrt k\quad\Longrightarrow\quad M\cong S_k^n.}
$$

This proves [maximal diameter rigidity from disjoint comparison balls](../../../../../../maximal-diameter-rigidity-from-disjoint-comparison-balls.md) directly, including the required equality argument.

**The literal trace interpretation again has a counterexample.** On $M=S^2(r)\times S^2(r)$ with $r^2=1/(2k)$, the [Ricci curvature](../../../../../../ricci-curvature.md) equals $2kg\geq kg$. For the [product Riemannian metric](../../../../../../product-riemannian-metric.md), distances satisfy $d^2=d_1^2+d_2^2$: every product curve has length at least $\sqrt{d_1^2+d_2^2}$ by the integral [triangle inequality](../../../../../../triangle-inequality.md), and a pair of constant-speed minimizing factor [geodesics](../../../../../../geodesic.md) attains it. Consequently

$$
\operatorname{diam}M=\sqrt{(\pi r)^2+(\pi r)^2}=\frac{\pi}{\sqrt k}.
$$

The mixed [sectional curvature](../../../../../../sectional-curvature.md) is zero, so this manifold is not $S_k^4$. The stronger bound, or [normalized Ricci curvature](../../../../../../normalized-ricci-curvature.md) convention, is essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
