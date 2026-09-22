<h1 id="16h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $T_f$ to consist of $T$ together with the following sentences.


- $f$ is injective and surjective:


$$
\forall x\,\forall y\,(f(x)=f(y)\Rightarrow x=y),
\qquad
\forall y\,\exists x\,f(x)=y.
$$


- For every $n$-ary operation symbol $\omega$ of $L$,


$$
\forall x_1\cdots\forall x_n\,
f(\omega(x_1,\ldots,x_n))
=\omega(f(x_1),\ldots,f(x_n)).
$$

This includes $f(c)=c$ for each constant symbol $c$.
- For every $n$-ary relation symbol $R$ of $L$,


$$
\forall x_1\cdots\forall x_n\,
\bigl(R(x_1,\ldots,x_n)\Longleftrightarrow
R(f(x_1),\ldots,f(x_n))\bigr).
$$

The first pair of axioms makes the interpretation $\vartheta$ a bijection. The remaining schemes say exactly that it preserves every operation and relation, so $(M,\vartheta)\models T_f$ exactly when $M\models T$ and $\vartheta\in\operatorname{Aut}(M)$.

Finally, $T$ is consistent and hence has a model $M$ by part (b). Expanding $M$ by interpreting $f$ as the identity automorphism gives a model of $T_f$, so $T_f$ is consistent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [16H](../../16h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
