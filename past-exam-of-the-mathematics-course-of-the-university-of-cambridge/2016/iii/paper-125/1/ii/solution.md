<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $T=(\theta,0)$, so $f(\theta)=0$, $K=\mathbb Q(\theta)$, and $f'(\theta)\ne0$. Let $[a]$ denote the class of $a\in K^*$ modulo squares. The required [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md) is

$$
\boxed{\alpha(O)=1,\qquad\alpha(P)=[x(P)-\theta]\ (P\ne O,T),\qquad\alpha(T)=[f'(\theta)].}
$$

The last value is needed in the domain only if $T\in E(\mathbb Q)$. Every displayed nonexceptional value is nonzero, because an affine point with $x=\theta$ necessarily has $y=0$ and equals $T$.

Consider a nonvertical line $y=mx+c$ whose three intersection points have $x$-coordinates $x_1,x_2,x_3$, counted with multiplicity. Since $f$ is monic,

$$
f(x)-(mx+c)^2=\prod_{i=1}^3(x-x_i).
$$

If none of these points is $T$, evaluating at $\theta$ gives

$$
\prod_{i=1}^3(x_i-\theta)=(m\theta+c)^2,
$$

and therefore the product of their $\alpha$-values is $1$ in the [square-class group](../../../../../../square-class-group-of-a-field.md). Tangencies are included by repeated factors. Since negation preserves the $x$-coordinate, this identity says $\alpha(P+Q)=\alpha(P)\alpha(Q)$.

If the line passes through $T$, put $f(x)=(x-\theta)g(x)$ and write the line as $y=m(x-\theta)$. The other two intersection abscissae $x_1,x_2$ satisfy

$$
g(x)-m^2(x-\theta)=(x-x_1)(x-x_2).
$$

Evaluating at $\theta$ now gives

$$
(x_1-\theta)(x_2-\theta)=g(\theta)=f'(\theta).
$$

Thus $\alpha(T)\alpha(P_1)\alpha(P_2)=[f'(\theta)]^2=1$, as required. This covers a tangent at a different point whose third intersection is $T$ as well.

The tangent at $T$ is vertical. For a vertical chord or tangent the two affine intersections are $P,-P$, so their product of [square classes](../../../../../../square-class.md) is $\alpha(P)^2=1$; in particular $\alpha(T)^2=1$ agrees with $2T=O$. Finally, adding $O$ changes neither side. These cases exhaust the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md), proving that the displayed map is a [group homomorphism](../../../../../../group-homomorphism.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
