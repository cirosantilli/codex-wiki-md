<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We first justify [surjectivity is preserved by base change](../../../../../../surjectivity-is-preserved-by-base-change.md) for [morphisms of schemes](../../../../../../morphism-of-schemes.md). Given $y'$ over $y$ and a point $x$ over $y$, the [fiber](../../../../../../fiber-of-a-function.md) after the residue-[field](../../../../../../field.md) extension contains a point because

$$
\kappa(x)\otimes_{\kappa(y)}\kappa(y')\ne0.
$$

Indeed, tensoring a nonzero [vector space](../../../../../../vector-space-split.md) over a [field](../../../../../../field.md) with a [field extension](../../../../../../field-extension.md) remains nonzero; a nonzero commutative [ring](../../../../../../ring.md) has a [prime ideal](../../../../../../prime-ideal.md), giving the required point. Thus every [base change](../../../../../../base-change-of-a-morphism-of-schemes.md) of $f$ is surjective.

Now make an arbitrary [base change](../../../../../../base-change-of-a-morphism-of-schemes.md) $Z'\to Z$. For a closed subset $C\subseteq Y'=Y\times_ZZ'$, its inverse image under $f':X'\to Y'$ is closed. The [proper morphism](../../../../../../proper-morphism.md) $(gf)':X'\to Z'$ therefore has closed image on that inverse image. Surjectivity of $f'$ gives

$$
g'(C)=(g'f')\bigl((f')^{-1}(C)\bigr),
$$

so $g'(C)$ is closed. This proves that $g$ is a [universally closed morphism](../../../../../../universally-closed-morphism.md). Together with the given [separatedness](../../../../../../separated-morphism.md) and [finite type](../../../../../../morphism-of-finite-type.md), it proves

$$
\boxed{gf\text{ proper},\ f\text{ surjective},\ g\text{ separated and of finite type}\ \Longrightarrow\ g\text{ proper}.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
