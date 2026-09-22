<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First use the [algebraically closed field](../../../../../../algebraically-closed-field.md) convention. Every [line bundle](../../../../../../line-bundle.md) on a [smooth projective curve](../../../../../../smooth-projective-curve.md) has a nonzero [rational section of a line bundle](../../../../../../rational-section-of-a-line-bundle.md): trivialize it on a nonempty open set and take its generic generator. The orders of its zeros and poles give a finite [divisor](../../../../../../divisor.md) $D$, and the local trivializations identify the [line bundle](../../../../../../line-bundle.md) with $\mathcal O(D)$. For a degree-zero [line bundle](../../../../../../line-bundle.md) write

$$
D=\sum_p n_pp,\qquad \sum_p n_p=0,
$$

since every closed point is a $k$-point. Therefore

$$
D=\sum_p n_p(p-p_0),\qquad
\mathcal O(D)\cong\bigotimes_p\mathcal O(p-p_0)^{\otimes n_p}.
$$

Only finitely many factors occur, and negative tensor powers mean dual [line bundles](../../../../../../line-bundle.md). This proves

$$
\boxed{\operatorname{Pic}^0(X)=\langle\alpha(X(k))\rangle.}
$$

For genus zero the group is trivial, so the conclusion remains valid.

For a general field, a closed point need not be rational, and its contribution to degree is weighted by its residue degree. Consequently **rational points need not generate the [degree-zero Picard group of a curve](../../../../../../degree-zero-picard-group-of-a-curve.md)**. Here is an explicit counterexample to that stronger reading. Let $C$ be the [smooth projective curve](../../../../../../smooth-projective-curve.md) over $\mathbb F_2$ obtained by completing the affine equation

$$
y^2+y=x^5+x+1.
$$

The polynomial is irreducible over $\overline{\mathbb F}_2(x)$: a function $r^2+r$ has even pole order at infinity when it has a pole there, while the right side has pole order five. Its affine model is smooth because the partial [derivative](../../../../../../derivative.md) with respect to $y$ is one. The normalized projective completion is therefore a geometrically integral [smooth projective curve](../../../../../../smooth-projective-curve.md).

There is exactly one point $p_\infty$ above infinity, and it is rational. Indeed the map $x:C\to\mathbb P^1$ has degree two. At a point above infinity put $v(x)=-e$, where the ramification index $e$ is at most two. The equation forces $v(y)<0$ and $2v(y)=5v(x)=-5e$. Hence $e=2$ and $v(y)=-5$. The degree formula then leaves exactly one point of residue degree one. Thus $x$ and $y$ have pole orders two and five there. There are no affine rational points: for either $x\in\mathbb F_2$, the right side is one, while $y^2+y=0$ for every $y\in\mathbb F_2$. Hence $C(\mathbb F_2)=\{p_\infty\}$ and the image of its [Abel map of a pointed smooth projective curve](../../../../../../abel-map-of-a-pointed-smooth-projective-curve.md) is trivial.

The equations $y=0$, $x^2+x+1=0$ define a degree-two closed point $D$, since $x^5+x+1$ vanishes modulo $x^2+x+1$. The [divisor](../../../../../../divisor.md) $D-2p_\infty$ has degree zero but is not principal. To prove this, a function with poles bounded by $2p_\infty$ is regular on the affine curve and hence has a unique expression $A(x)+B(x)y$. The possible pole orders of its two terms are $2\deg A$ and $2\deg B+5$, of opposite parity, so they cannot cancel. The pole bound forces $B=0$ and $\deg A\le1$. But no nonzero $a+bx$ over $\mathbb F_2$ vanishes at $D$, whose residue class of $x$ has irreducible quadratic minimal polynomial. Thus no function has [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) $D-2p_\infty$, proving its class is nonzero. This establishes the [rational points need not generate the degree-zero Picard group](../../../../../../rational-points-need-not-generate-the-degree-zero-picard-group.md) qualification with a complete obstruction, while the generation proof above supplies the intended algebraically closed-field answer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
