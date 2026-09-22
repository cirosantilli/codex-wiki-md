<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the equation as $\epsilon x^3-(x-1)^2=0$. For $\epsilon\to0^+$, two [roots of a polynomial](../../../../root-of-a-polynomial.md) approach the double root one. Their splitting follows a fractional-power [dominant balance](../../../../dominant-balance.md), rather than an ordinary expansion in integer powers.

Put $\delta=\sqrt\epsilon$ and $x=1+a\delta+b\delta^2+\cdots$. Substitution gives

$$
0=(1-a^2)\delta^2+(3a-2ab)\delta^3+O(\delta^4).
$$

Thus $a=\pm1$ and $b=3/2$. The two bounded roots have the [Puiseux series](../../../../puiseux-series.md) expansions

$$
\boxed{x_\pm=1\pm\sqrt\epsilon+\frac32\epsilon+O(\epsilon^{3/2}).}
$$

The first two nonzero terms are $1\pm\sqrt\epsilon$; the displayed correction also resolves their common order-$\epsilon$ shift.

The third root escapes to infinity because the leading [polynomial degree](../../../../degree-of-a-polynomial.md) drops when $\epsilon=0$. Balance $\epsilon x^3$ against $x^2$, giving $x=O(\epsilon^{-1})$. Set $X=\epsilon x$; the equation becomes

$$
X^3-X^2+2\epsilon X-\epsilon^2=0.
$$

For $X=1+A\epsilon+B\epsilon^2+\cdots$, the first two coefficient equations are $A+2=0$ and $B+2A^2+2A-1=0$. Hence

$$
\boxed{x_\infty=\epsilon^{-1}-2-3\epsilon+O(\epsilon^2).}
$$

Its first two nonzero terms are $\epsilon^{-1}-2$. These three distinct branches account for all roots of the cubic for sufficiently small positive $\epsilon$. The [Vieta formulas](../../../../vieta-s-formulas.md) provide a consistency check: their sum is $\epsilon^{-1}$, with the constant and order-$\epsilon$ terms cancelling.

If $\epsilon$ approaches zero through negative values, the bounded pair is complex: $x_\pm=1\pm i\sqrt{|\epsilon|}+\tfrac32\epsilon+O(|\epsilon|^{3/2})$. The large-root expansion is unchanged as a real asymptotic formula. The positive-parameter regime is used for the boundary-layer problem below.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
