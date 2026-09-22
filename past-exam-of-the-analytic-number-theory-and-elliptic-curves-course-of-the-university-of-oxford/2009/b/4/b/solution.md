<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The three suggested values are

$$
h(-2)=-7,\qquad h(0)=-1,\qquad h(3)=23.
$$

There is an obstruction at $p=3$: every [integer](../../../../../integer-split.md) residue satisfies $x^3-x\equiv0\pmod3$, whereas $-1\equiv2$ is not a square modulo three. Reduction of a solution in the [p-adic integers](../../../../../p-adic-integer.md) would give an impossible solution modulo three.

At $p=2$, take $x=-2$. The odd 2-adic [unit in a ring](../../../../../unit-in-a-ring.md) $-7$ is congruent to one modulo eight, so it is a square in $\mathbb Z_2$. We use the standard 2-adic square criterion that an odd [unit in a ring](../../../../../unit-in-a-ring.md) is a square exactly when it is one modulo eight. Its sufficiency follows by successively adjusting an odd square root modulo $2^m$ by $2^{m-1}$ to obtain the next required square congruence. Thus $y^2=-7$ has a 2-adic [integer](../../../../../integer-split.md) solution.

For $p\geq5$ other than $23$, the discriminant of $y^2=x^3-x-1$ is

$$
\Delta=-16\bigl(4(-1)^3+27(-1)^2\bigr)=-16\cdot23,
$$

so this model has [good reduction of an elliptic curve](../../../../../good-reduction-of-an-elliptic-curve.md). [Hasse's theorem on elliptic curves](../../../../../hasse-s-theorem-on-elliptic-curves.md) gives

$$
\#E(\mathbb F_p)\geq p+1-2\sqrt p>1.
$$

Since there is just one point at infinity, there is an affine point. Smoothness means that at least one partial derivative of $y^2-x^3+x+1$ is a [unit in a ring](../../../../../unit-in-a-ring.md) modulo $p$, so [Hensel's lemma](../../../../../hensel-s-lemma.md) lifts the affine point to $\mathbb Z_p^2$. The last exceptional odd [prime](../../../../../prime-number-split.md) is also soluble: at $p=23$, $h(-2)=-7\equiv16$ has square roots $\pm4$, which are simple roots of $Y^2+7$ modulo $23$, and lift by [Hensel's lemma](../../../../../hensel-s-lemma.md).

For small-prime checks the suggested values also give $x=0$ at $p=5$ and $x=3$ at $p=7$, where respectively $-1\equiv2^2$ and $23\equiv3^2$. Therefore

$$
\boxed{\text{a solution in }\mathbb Z_p^2\text{ exists exactly when }p\neq3.}
$$

The same [prime](../../../../../prime-number-split.md) list holds if one only asks for a solution modulo $p$, but the lifting above establishes the asserted [p-adic integer](../../../../../p-adic-integer.md) solutions. This is [local solubility of the cubic x cubed minus x minus one](../../../../../local-solubility-of-the-cubic-x-cubed-minus-x-minus-one.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
