<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual essential two-person [Nash bargaining problem](../../../../../../nash-bargaining-problem.md): $F\subset\mathbb R^2$ is a [compact convex set](../../../../../../compact-convex-set.md), $d\in F$ is the [disagreement point](../../../../../../disagreement-point.md), and some $u\in F$ satisfies $u_i>d_i$ for both players. The [Nash bargaining solution](../../../../../../nash-bargaining-solution.md) is

$$
\boxed{N(F,d)=\mathop{\operatorname{argmax}}_{u\in F,\ u\geq d}
(u_1-d_1)(u_2-d_2).}
$$

The positive maximum exists by compactness and essentiality. On positive gains, maximizing this [Nash product](../../../../../../nash-product.md) is equivalent to maximizing $\log(u_1-d_1)+\log(u_2-d_2)$, a [strictly concave function](../../../../../../strictly-concave-function.md). Convexity then gives a unique maximizer. The essentiality and compactness hypotheses matter: for example, with $F=[0,1]\times\{0\}$ and $d=0$, the product is zero everywhere and its argmax alone is not a single-valued definition.

The rule satisfies all four axioms. **[Pareto efficiency](../../../../../../pareto-efficiency.md):** a feasible vector dominating the chosen vector with at least one strict improvement would increase its positive [Nash product](../../../../../../nash-product.md). **[Bargaining symmetry](../../../../../../bargaining-symmetry.md):** if the problem is unchanged by swapping players, uniqueness makes the answer unchanged, so the two payoffs agree. **[Positive affine invariance in bargaining](../../../../../../positive-affine-invariance-in-bargaining.md):** for $v_i=a_i u_i+b_i$ with $a_i>0$, gains transform to $a_i(u_i-d_i)$ and the product is multiplied by the positive constant $a_1a_2$, preserving its maximizer. **[Bargaining independence of irrelevant alternatives](../../../../../../bargaining-independence-of-irrelevant-alternatives.md):** if $G\subseteq F$ is another admissible feasible set containing the chosen vector and the same disagreement point, that vector remains the unique product maximizer over $G$.

To prove characterization, let $f$ be any feasible single-valued rule satisfying these axioms, and let $u^*=N(F,d)$. Normalize payoffs by the positive affine transformation

$$
z_i=\frac{u_i-d_i}{u_i^*-d_i}.
$$

The transformed set $H$ has disagreement point zero and product maximizer $e=(1,1)$. For any $z\in H$, convexity puts $e+t(z-e)$ in $H$; for sufficiently small $t>0$ both gains remain positive. The one-sided [derivative](../../../../../../derivative.md) of the product at its maximum is therefore nonpositive:

$$
\left.\frac{d}{dt}\prod_{i=1}^2(1+t(z_i-1))\right|_{t=0}
=z_1+z_2-2\leq0.
$$

Thus $H\subseteq\{z:z_1+z_2\leq2\}$. By compactness choose $M\geq0$ so every coordinate of every $z\in H$ is at least $-M$. The [supporting triangle for Nash bargaining](../../../../../../supporting-triangle-for-nash-bargaining.md) is

$$
T_M=\{z:z_1\geq-M,\ z_2\geq-M,\ z_1+z_2\leq2\}.
$$

It contains $H$, is compact, convex, symmetric and essential, and contains disagreement zero. Symmetry forces $f(T_M,0)$ onto the diagonal; [Pareto efficiency](../../../../../../pareto-efficiency.md) then forces it to be $e=(1,1)$. Since $e\in H\subseteq T_M$, [bargaining independence of irrelevant alternatives](../../../../../../bargaining-independence-of-irrelevant-alternatives.md) gives $f(H,0)=e$. Undoing the normalization by [positive affine invariance in bargaining](../../../../../../positive-affine-invariance-in-bargaining.md) gives $f(F,d)=u^*$. Hence the four axioms uniquely characterize the [Nash bargaining solution](../../../../../../nash-bargaining-solution.md) on this domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
