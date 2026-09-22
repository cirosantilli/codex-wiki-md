<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $m=2n$ and let $\alpha$ be the identity class of $S^m$. With the product-cell orientation used in part (i), form the folding map $\nabla:S^m\vee S^m\to S^m$, which is identity on each summand. The top cell of $S^m\times S^m$ is attached by the product of the two inclusions, so folding gives the attaching map $[\alpha,\alpha]_W$. Thus there is a [cellular map](../../../../../../cellular-map.md)

$$
F:S^m\times S^m\longrightarrow C,
\qquad C=S^m\cup_{[\alpha,\alpha]_W}D^{2m},
$$

which is the fold on the lower skeleton and degree one on the top relative cell.

Let $a,b\in H^m(S^m\times S^m;\mathbb Z)$ be the classes from the two factors, and let $x\in H^m(C;\mathbb Z)$ restrict to the generator of the bottom sphere. Orient the top class $z\in H^{2m}(C;\mathbb Z)$ so that $F^*z=ab$. Then $F^*x=a+b$. Since $a^2=b^2=0$ and $m$ is even, [graded commutative algebra](../../../../../../graded-commutative-algebra.md) gives

$$
F^*(x^2)=(a+b)^2=ab+ba=2ab=F^*(2z).
$$

The map $F^*$ is an isomorphism in degree $2m$, because of its degree-one top-cell map. Therefore $x^2=2z$. By the definition of the [Hopf invariant](../../../../../../hopf-invariant.md) this proves

$$
\boxed{H([\alpha,\alpha])=2.}
$$

The shifted Lie convention in part (i) multiplies the geometric bracket by $(-1)^m=1$, so it gives the same square and the same invariant. Reversing the orientation chosen for the attached top cell would reverse both its generator and the numerical sign convention; with the standard orientation the value is the stated positive two.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
