<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $q=1-2r/\sigma^2$. The [Black-Scholes reflection symmetry](../../../../../black-scholes-reflection-symmetry.md) maps $F$ to $(S/B)^qF(B^2/S,t)$, which solves the same PDE. Their difference vanishes at $S=B$. For $S>B$ at maturity the reflected argument is below $B$, where the terminal function in part [ii](../ii.md) is zero. Thus the boundary and terminal data of the alive [down-and-out put](../../../../../down-and-out-put.md) are satisfied:

$$
\boxed{G(S,t)=F(S,t)-\left(\frac SB\right)^qF(B^2/S,t),\qquad S>B.}
$$

The killed-domain [Feynman-Kac formula](../../../../../feynman-kac-formula.md) identifies this solution with the discounted payoff conditional on survival. For $S\leq B$, or after any prior barrier hit, the actual price is **zero**. The reflected difference is a formula on the alive domain $S>B$; extending that algebraic expression to $S<B$ generally gives a nonzero, possibly negative function and is not a valid barrier-option price.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
