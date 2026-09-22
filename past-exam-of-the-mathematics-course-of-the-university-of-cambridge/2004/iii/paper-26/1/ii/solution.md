<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Start from the [integral triangular basis of level-one modular forms](../../../../../../integral-triangular-basis-of-level-one-modular-forms.md). Proceed downwards in $j$. Set $g_{d-1}=F_{d-1}$; once $g_{j+1},\ldots,g_{d-1}$ are constructed, subtract from $F_j$ its coefficients at $q^{j+1},\ldots,q^{d-1}$ times these respective forms. The already constructed rows have a single nonzero coefficient among those initial positions, so this removes every unwanted initial coefficient without changing the coefficient one at $q^j$. All subtractions use integers. The resulting [integral echelon basis of level-one modular forms](../../../../../../integral-echelon-basis-of-level-one-modular-forms.md) therefore has

$$
\boxed{g_j=q^j+\sum_{n\geq d}c_n(j)q^n,\qquad c_n(j)\in\mathbb Z.}
$$

Its first $d$ coefficient vectors are the standard coordinate vectors, hence it is a basis. If another form had the same first $d$ coefficients as $g_j$, their difference would have those coefficients all zero; the triangular basis proves that difference vanishes. This proves uniqueness of every $g_j$, not merely uniqueness up to basis change.

For any $f\in M_k$, its expansion in this basis is $f=\sum_{j=0}^{d-1}a_j(f)g_j$, since its first $d$ coefficients determine the basis coordinates. Comparing subsequent coefficients gives

$$
\boxed{a_n(f)=\sum_{j=0}^{d-1}c_n(j)a_j(f),\qquad n\geq d.}
$$

The coefficients of $f$ need not be integral for this last identity. When needed at earlier indices, extend the notation by $c_n(j)=\delta_{nj}$ for $0\leq n<d$. This agrees with the actual coefficients of the basis forms and is the convention needed for the next part's all-index wording.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
