<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

For a [smooth projective curve](../../../../../smooth-projective-curve.md) of [genus](../../../../../genus-of-a-surface.md) $g$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) states

$$
\ell(D)-\ell(K-D)=\deg D+1-g,
$$

where $D$ is a [divisor](../../../../../divisor.md), $K$ a [canonical divisor](../../../../../canonical-divisor.md), and $\ell(D)=\dim H^0(V,\mathcal O_V(D))$. In particular, applying it to $D=0$ and $D=K$ gives $\ell(K)=g$ and $\deg K=2g-2$.

For a nonconstant morphism $f:C\to D$ of degree $d$ in characteristic zero, choose local parameters with $t\circ f=u^e$ up to a unit at a point of [ramification index](../../../../../ramification-index.md) $e$. Pulling back a differential multiplies its local order by $e$ and adds $e-1$, because $d(u^e)=eu^{e-1}du$ and $e\ne0$ in the field. Thus

$$
K_C\sim f^*K_D+\sum_{P\in C}(e_P-1)P.
$$

The [degree of a divisor](../../../../../degree-of-a-divisor.md) of a pulled-back [divisor](../../../../../divisor.md) is $d$ times its degree. Taking degrees and using the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md)

$$
\boxed{2g_C-2=d(2g_D-2)+\sum_P(e_P-1).}
$$

A smooth plane cubic has [genus](../../../../../genus-of-a-surface.md) one by the [genus-degree formula](../../../../../genus-degree-formula.md). In the displayed normal form, $F(0,X_1)=cX_1^3$ with $c\ne0$: otherwise $X_0$ divides $F$ and the cubic is reducible. Therefore the line $X_0=0$ meets the cubic in the [divisor](../../../../../divisor.md) $3P_0$, and $\mathcal O_V(1)\cong\mathcal O_V(3P_0)$. The [elliptic curve](../../../../../elliptic-curve.md) group law identifies $P$ with the degree-zero [divisor](../../../../../divisor.md) class $[P-P_0]$. Order three means $3P\sim3P_0$. Consequently $\mathcal O_V(3P)\cong\mathcal O_V(1)$ and has a section with zero [divisor](../../../../../divisor.md) $3P$.

Every section of $\mathcal O_V(1)$ is the restriction of a linear form: ambient linear forms form a three-dimensional space and restrict injectively, while [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal O_V(1))=3$, since $\deg(K-3P_0)=-3$ forces the dual term to vanish. Thus this section is some nonzero $H$, proving **$V\cap V(H)=\{P\}$, with intersection multiplicity three**. This is the [three-torsion points are flexes of a plane cubic](../../../../../three-torsion-points-are-flexes-of-a-plane-cubic.md) property.

Projection forgetting $X_3$ defines a morphism $W\to V$: its only possible indeterminacy point $(0:0:0:1)$ does not satisfy the second equation. It is a double cover. Away from the zeros of $H_1H_2$, its two square roots are distinct. Each line intersects $V$ in three simple points, since it is nowhere tangent; the two triples are disjoint because the lines do not meet on $V$. In a local trivialization near any of these six points the covering equation is $s^2=u\,a(u)$ with $a(0)\ne0$, so the [ramification index](../../../../../ramification-index.md) is two. There is no other ramification. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) therefore gives

$$
2g_W-2=2(2\cdot1-2)+6=6,\qquad\boxed{g_W=4.}
$$

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
