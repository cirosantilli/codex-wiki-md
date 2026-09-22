<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u'$ be any constrained minimizer for $\sigma>0$ and let $\lambda^*$ be a dual optimum. Set the common optimal value to $p^*$. [Weak duality](../../../../../../weak-duality.md) and feasibility imply

$$
p^*=d(\lambda^*)\leq L(u',\lambda^*)
=\operatorname{TV}(u')+\lambda^*(r(u')-\sigma)\leq\operatorname{TV}(u')=p^*.
$$

All inequalities are therefore equalities. In particular, $u'$ minimizes $L(\cdot,\lambda^*)$, whose $-\lambda^*\sigma$ term is constant. Hence

$$
\boxed{u'\in\operatorname*{argmin}_u\{\operatorname{TV}(u)+\lambda^*\|u-g\|_2^2\},\qquad\lambda^*\geq0.}
$$

This proves the claim for every constrained minimizer, rather than just for the particular one used to establish a saddle point. The multiplier may be zero, and the penalized minimizer then need not be unique.

Conversely, for $\lambda>0$ the quadratic makes the penalized objective coercive and strictly convex, so it has a unique minimizer $u_\lambda$. Choose $\boxed{\sigma=\|u_\lambda-g\|_2^2}$. If a feasible $u$ had $\operatorname{TV}(u)<\operatorname{TV}(u_\lambda)$, then

$$
\operatorname{TV}(u)+\lambda r(u)
\leq\operatorname{TV}(u)+\lambda\sigma
<\operatorname{TV}(u_\lambda)+\lambda r(u_\lambda),
$$

contradicting penalized optimality. Thus $u_\lambda$ solves the constrained problem at that budget. This is [constrained-penalized equivalence for total variation denoising](../../../../../../constrained-penalized-equivalence-for-total-variation-denoising.md). It is a correspondence of minimizers and suitable parameters, not a claim that every budget has a unique multiplier or a unique constrained minimizer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
