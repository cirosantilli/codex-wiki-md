<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The real [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) says that if $C$ is a nonempty open [convex set](../../../../../convex-set-split.md) in a real [normed vector space](../../../../../normed-vector-space-split.md) and $y\notin C$, there is a nonzero [continuous linear functional](../../../../../continuous-linear-functional.md) $g$ such that $g(y)\geq\sup_{z\in C}g(z)$.

Put $\delta=1-1/M\in(0,1)$. The prescribed set is open because it is a union of translates of an open ball, and it is [convex](../../../../../convex-function.md) because both summands are [convex](../../../../../convex-function.md). If $\|y\|<1$ and $y\notin C$, [Hahn-Banach separation](../../../../../hahn-banach-separation-theorem.md) gives a nonzero $g\in Y^*$ with

$$
g(y)\geq\sup_{z\in C}g(z)=\|T^*g\|+\delta\|g\|\geq(M^{-1}+\delta)\|g\|=\|g\|.
$$

The displayed supremum is a sum of independent suprema; the symmetry of the unit balls identifies them with the respective [operator norms](../../../../../operator-norm.md). But $g(y)\leq\|g\|\|y\|<\|g\|$, a contradiction. Hence $y=Tx+r$ for some $\|x\|\leq1$ and $\|r\|<\delta$.

To obtain the strict bound on $x$ required in the approximation hypothesis, choose $t<1$ sufficiently close to $1$. Then $\|tx\|<1$ and

$$
\|T(tx)-y\|\leq\|r\|+(1-t)\|Tx\|<\delta.
$$

Thus the approximation condition holds with exactly $\delta=1-1/M$. When $X$ is a [Banach space](../../../../../banach-space-split.md), the preceding [successive approximation for quotient operators](../../../../../successive-approximation-for-quotient-operators.md) proves $T$ is a [quotient operator](../../../../../quotient-operator.md). Combining this with the [Banach-space adjoint](../../../../../transpose-of-a-bounded-linear-operator.md) estimate proves

$$
\boxed{T\text{ is a quotient operator}\iff T^*\text{ is an isomorphic embedding}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
