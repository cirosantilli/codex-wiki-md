<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In Siegel's original convention, an [E-function](../../../../../../e-function.md) is an entire series $F(z)=\sum_{n\ge0}a_nz^n/n!$ with coefficients in a fixed [number field](../../../../../../number-field.md), satisfying a nonzero [linear differential equation](../../../../../../linear-differential-equation.md) over $\overline{\mathbb Q}(z)$, together with these arithmetic bounds: for every $\epsilon>0$, all conjugates of $a_0,\ldots,a_n$ have size $O_\epsilon(n^{\epsilon n})$, and some positive [integer](../../../../../../integer.md) $d_n=O_\epsilon(n^{\epsilon n})$ makes every $d_na_j$, $j\le n$, an [algebraic integer](../../../../../../algebraic-integer.md). A frequently used stricter convention replaces both bounds by $C^{n+1}$. The original and strict growth definitions should not simply be declared equivalent; the exponential examples below satisfy the strict one.

For sums, work in the [compositum](../../../../../../field-compositum.md) of the coefficient fields. Coefficient conjugate bounds add. The product of the two common denominators clears both lists; using $\epsilon/2$ in each original denominator bound gives the required $O_\epsilon(n^{\epsilon n})$ product bound. Finally all derivatives of $F+G$ lie in the sum of the two finite-dimensional derivative spaces over that [rational function](../../../../../../rational-function.md) [field](../../../../../../field.md), so they satisfy a nontrivial [linear dependence](../../../../../../linear-dependence.md), giving a differential equation for the sum. Thus **sums are again E-functions**, the [addition closure of Siegel E-functions](../../../../../../addition-closure-of-siegel-e-functions.md).

The [Siegel–Shidlovsky theorem](../../../../../../siegel-shidlovsky-theorem.md) states that if a vector of E-functions satisfies $F'=A(z)F$ with rational-function matrix over $\overline{\mathbb Q}$, then at every nonzero algebraic $\xi$ which is not a pole of $A$,

$$
\operatorname{trdeg}_{\overline{\mathbb Q}}\overline{\mathbb Q}(F_1(\xi),\ldots,F_s(\xi))=\operatorname{trdeg}_{\overline{\mathbb Q}(z)}\overline{\mathbb Q}(z)(F_1(z),\ldots,F_s(z)).
$$

In particular algebraically independent functions give algebraically independent values.

Take $F_j(z)=e^{\gamma_jz}$ for [algebraic numbers](../../../../../../algebraic-number.md) $\gamma_j$ linearly independent over $\mathbb Q$. Their coefficients are $\gamma_j^n$ with exponential conjugate and denominator bounds, and $F_j'=\gamma_jF_j$. A [polynomial](../../../../../../polynomial-split.md) relation among the functions expands into a relation among exponentials with distinct exponents $\sum m_j\gamma_j$ and [polynomial](../../../../../../polynomial-split.md) coefficients after clearing rational-function denominators; exponential-polynomial independence excludes it. At $\xi=1$ the theorem gives [algebraic independence](../../../../../../algebraic-independence.md) of the $e^{\gamma_j}$. For arbitrary distinct algebraic $\alpha_i$, choose a rational basis of their span and divide that basis by a common denominator. The $e^{\alpha_i}$ are distinct Laurent monomials in the corresponding algebraically independent exponential values, so are linearly independent over $\overline{\mathbb Q}$. This recovers the general [Lindemann–Weierstrass theorem](../../../../../../lindemann-weierstrass-theorem.md). Its simplest instance uses just $F(z)=e^z$ at nonzero algebraic $\xi$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
