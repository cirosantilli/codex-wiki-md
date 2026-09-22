<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [down-and-out digital call](../../../../../down-and-out-digital-call.md) with strike at the barrier pays one exactly when the barrier is avoided until expiry. Reflection therefore gives its alive price

$$
D_{\mathrm{out}}(S,t)=C_d(S,t;B)-\left(\frac SB\right)^qC_d(B^2/S,t;B),\qquad S>B.
$$

The complementary contract pays one at expiry when the barrier has been hit. Its price is

$$
\boxed{H(t,S)=e^{-r\tau}-D_{\mathrm{out}}(S,t),\qquad S>B\text{ and no previous hit}.}
$$

This is a cash-at-expiry [one-touch option](../../../../../one-touch-option.md), not cash paid at the first touch. After the barrier has already been hit, its price is $e^{-r\tau}$ regardless of the current spot. In particular this branch applies immediately for $S\leq B$. Current spot alone does not encode the full path history.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
