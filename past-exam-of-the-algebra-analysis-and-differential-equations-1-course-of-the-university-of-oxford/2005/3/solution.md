<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [ideal](../../../ideal.md) is an additive subgroup of a [ring](../../../ring.md) closed under multiplication by arbitrary ring elements; in a potentially noncommutative ring, a two-sided ideal must absorb multiplication on both sides. For a [ring homomorphism](../../../ring-homomorphism.md) $\phi$, its [kernel of a ring homomorphism](../../../kernel-of-a-ring-homomorphism.md) $K=\{r:\phi(r)=0\}$ contains zero, is closed under subtraction, and satisfies $\phi(rk)=\phi(r)\phi(k)=0$ and $\phi(kr)=0$. Thus $K$ is an ideal.

Define $\widetilde\phi:R/K\to S$ by $r+K\mapsto\phi(r)$. It is well-defined because two representatives differ by an element of $K$, preserves addition and multiplication, is surjective by hypothesis, and is injective because its zero class is precisely $K$. Therefore $\boxed{R/\ker\phi\cong S}$, the [first isomorphism theorem for rings](../../../first-isomorphism-theorem-for-rings.md).

Apply this to the [evaluation homomorphism](../../../evaluation-homomorphism.md) $\mathbb C[z]\to\mathbb C$, $p\mapsto p(1)$. Constants prove surjectivity, and division by $z-1$ shows that its [kernel of a ring homomorphism](../../../kernel-of-a-ring-homomorphism.md) is $(z-1)$. Hence $\boxed{\mathbb C[z]/(z-1)\cong\mathbb C}$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2005](../../2005-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
