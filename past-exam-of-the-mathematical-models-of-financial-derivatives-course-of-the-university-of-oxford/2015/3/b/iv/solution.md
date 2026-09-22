<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $0<B<K$, every surviving terminal price is already below the strike, so this is a [barrier digital put](../../../../../barrier-digital-put.md) paying one at expiry exactly when the upper barrier has been avoided. To use the [Black-Scholes reflection symmetry](../../../../../black-scholes-reflection-symmetry.md), cap the free digital-put strike at $B$, rather than continuing to use $K$:

$$
\boxed{H(S,t)=D_B(S,t)-(S/B)^\gamma D_B(B^2/S,t),\qquad0<S<B<K.}
$$

Indeed, $D_B$ has terminal payoff one throughout the alive region, while its reflected argument exceeds $B$ and hence has zero terminal payoff. The barrier values again cancel. Using $D_K$ in both terms would generally leave an unwanted reflected terminal payoff near the barrier.

Writing $b=r-\sigma^2/2$ makes the discounted survival [probability](../../../../../probability.md) explicit:

$$
\boxed{H(S,t)=e^{-r\tau}\left[
\Phi\!\left(\frac{\log(B/S)-b\tau}{\sigma\sqrt\tau}\right)
-(S/B)^\gamma\Phi\!\left(\frac{\log(S/B)-b\tau}{\sigma\sqrt\tau}\right)
\right].}
$$

The price is independent of $K$ in this case. Both cases combine by replacing the free strike with $\min(K,B)$ in the [up-and-out digital put](../../../../../up-and-out-digital-put.md) formula.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
