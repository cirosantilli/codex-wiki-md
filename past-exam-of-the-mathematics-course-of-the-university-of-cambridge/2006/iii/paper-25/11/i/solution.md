<h1 id="11/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [Ehrenfeucht-Mostowski theorem](../../../../../../ehrenfeucht-mostowski-theorem.md) by [ultraproducts](../../../../../../ultraproduct.md), with no application of [Ramsey theorem](../../../../../../ramsey-theorem.md). Expand the infinite structure $M$ by [Skolem functions](../../../../../../skolem-function.md), choose distinct elements $a_0,a_1,\ldots$, and choose a [nonprincipal ultrafilter](../../../../../../nonprincipal-ultrafilter.md) $D$ on $\omega$. Let $I$ be the desired total index order and put $J=\omega^I$.

For every finite ordered [subset](../../../../../../subset.md) $F=\{i_1<\cdots<i_n\}$, define an [ultrafilter](../../../../../../ultrafilter.md) $D_F$ on $\omega^F$ by the ordered [Fubini product of ultrafilters](../../../../../../fubini-product-of-ultrafilters.md): a [set](../../../../../../set-split.md) $B$ belongs to $D_F$ exactly when

$$
(Dm_1)(Dm_2)\cdots(Dm_n)\quad (m_1,\ldots,m_n)\in B.
$$

Here $(Dm)\psi(m)$ means $\{m:\psi(m)\}\in D$, with the quantifiers nested in the displayed order. The resulting collection is an [ultrafilter](../../../../../../ultrafilter.md), by induction using the [ultrafilter](../../../../../../ultrafilter.md) laws for negation and conjunction. For $F\subseteq H$, the inverse image of $B\subseteq\omega^F$ under coordinate projection belongs to $D_H$ exactly when $B\in D_F$: quantifiers on unused coordinates leave a truth value unchanged.

Consequently there is a well-defined [ultrafilter](../../../../../../ultrafilter.md) on the [Boolean algebra](../../../../../../boolean-algebra.md) of finite-coordinate cylinders in $J$, declaring a cylinder large by this test. Coherence proves finite [intersection](../../../../../../set-intersection.md) closure and ensures that the empty cylinder is not large. Extend its generated filter to an [ultrafilter](../../../../../../ultrafilter.md) $U$ on all [subsets](../../../../../../subset.md) of $J$. Form the [ultrapower](../../../../../../ultrapower.md) $N=(M^*)^J/U$, and for $i\in I$ let $b_i$ be the class of $s\mapsto a_{s(i)}$.

If $i\ne j$, the coordinate equality test belongs to no corresponding two-coordinate product [ultrafilter](../../../../../../ultrafilter.md): for every value of the outer coordinate, the inner equality [set](../../../../../../set-split.md) is a [singleton](../../../../../../singleton-mathematics.md), excluded by nonprincipality. Hence the $b_i$ are distinct. For any [first-order formula](../../../../../../first-order-formula.md) $\varphi(x_1,\ldots,x_n)$ and any $i_1<\cdots<i_n$, the [Łoś theorem](../../../../../../los-theorem.md) gives

$$
N\models\varphi(b_{i_1},\ldots,b_{i_n})
\quad\Longleftrightarrow\quad
(Dm_1)\cdots(Dm_n)\ M^*\models\varphi(a_{m_1},\ldots,a_{m_n}).
$$

The right side is independent of the actual increasing index tuple, so the $b_i$ form an [order-indiscernible sequence](../../../../../../order-indiscernible-sequence.md). Constant [functions](../../../../../../function-split.md) embed $M^*$ elementarily into $N$. Take the [Skolem hull](../../../../../../skolem-hull.md) of the generators. The [Tarski-Vaught test](../../../../../../tarski-vaught-test.md) gives an [elementary substructure](../../../../../../elementary-substructure.md), and transporting terms along an index-order automorphism gives a well-defined automorphism of the hull, with inverse obtained by transporting along the inverse index automorphism. Equality of term representations is preserved by indiscernibility. **This is the indiscernible and automorphism conclusion of Ehrenfeucht–Mostowski, obtained entirely from [ultrafilters](../../../../../../ultrafilter.md) and Łoś's theorem.** The ordered Fubini products need not be symmetric; order indiscernibility is exactly what their coherence supplies.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11](../../11.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
