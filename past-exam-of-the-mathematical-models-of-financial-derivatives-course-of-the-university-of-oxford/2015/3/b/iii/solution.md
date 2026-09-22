<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $D_K(S,t)=P_d(S,t)$ and $\gamma=1-2r/\sigma^2$. The [Black-Scholes reflection symmetry](../../../../../black-scholes-reflection-symmetry.md) gives another solution $(S/B)^\gamma D_K(B^2/S,t)$. Subtracting it enforces absorption:

$$
\boxed{H(S,t)=D_K(S,t)-(S/B)^\gamma D_K(B^2/S,t),\qquad0<S<B,\quad B>K.}
$$

At $S=B$ the terms agree. At expiry the reflected argument satisfies $B^2/S>B>K$, so its digital-put payoff vanishes; the first term supplies the required terminal payoff. These facts and the bounded pricing solution's uniqueness prove the formula. The [up-and-out digital put](../../../../../up-and-out-digital-put.md) price is zero once knocked out.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
