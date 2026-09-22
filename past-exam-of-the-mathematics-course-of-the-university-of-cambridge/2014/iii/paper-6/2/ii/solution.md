<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider the restriction operator

$$
T:X\longrightarrow E^*,\qquad (Tx)(e)=e(x),\qquad a=x^{**}|_E.
$$

It is onto: otherwise its range, a [vector subspace](../../../../../../vector-subspace.md) of the [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) $E^*$, would have a nonzero annihilator in $E^{**}=E$. That annihilator would be an $e\in E$ vanishing on all of $X$, so $e=0$, a contradiction. Moreover $T$ is open. To see this directly, choose preimages of a basis of $E^*$; they define a linear right inverse $S:E^*\to X$, continuous because its domain is finite-dimensional. Small changes of an image can then be lifted by small changes using $S$.

Put $r=1+\varepsilon$ and $C=T(\{x:\|x\|<r\})$. It is open and convex in $E^*$. If $a\notin C$, the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) gives a nonzero real [linear functional](../../../../../../linear-functional.md) on $E^*$, represented by some $e\in E$, such that

$$
a(e)\geq\sup_{z\in C}z(e)=r\|e\|.
$$

But $a(e)=x^{**}(e)\leq\|e\|$, contradicting $r>1$. Therefore $a\in C$, and the [finite-dimensional interpolation form of Goldstine's theorem](../../../../../../finite-dimensional-interpolation-form-of-goldstine-s-theorem.md) yields

$$
\boxed{\|x\|<1+\varepsilon,\qquad e(x)=x^{**}(e)\text{ for every }e\in E.}
$$

If $E=\{0\}$ one simply takes $x=0$.

To recover the [Goldstine theorem](../../../../../../goldstine-theorem.md), start with $x^{**}\in B_{X^{**}}$ and finitely many tests $e_1,\ldots,e_m\in X^*$. Apply the result to their span with a small parameter $\delta>0$. The resulting $x$ need not lie in $B_X$, but $v=x/(1+\delta)$ does. For every test,

$$
|e_j(v)-x^{**}(e_j)|=\frac{\delta}{1+\delta}|x^{**}(e_j)|\leq\delta\|e_j\|.
$$

Choosing $\delta$ sufficiently small puts $Jv$ in any prescribed basic weak-star neighborhood. This proves the asserted weak-star density of the closed [unit ball](../../../../../../unit-ball.md). The reverse inclusion follows because $B_{X^{**}}$ is weak-star closed, being the intersection of the conditions $|x^{**}(e)|\leq\|e\|$ for $e\in X^*$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
