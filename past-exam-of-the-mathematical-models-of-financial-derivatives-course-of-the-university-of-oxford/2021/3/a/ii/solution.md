<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\tau_B=\inf\{u\geq t:S_u\leq B\}$. While the contract is alive, the [down-and-out put](../../../../../down-and-out-put.md) pays $(K-S_T)^+\mathbf1_{\{\tau_B>T\}}$ at maturity; a prior touch has already knocked it out.

The truncated terminal payoff can be represented by the ordinary European-price combination

$$
F(S,t):=C(S,t;K)-C(S,t;B)+(K-B)C_d(S,t;B).
$$

At maturity its three regions are

$$
\boxed{F(S,T)=(K-S)^+\mathbf1_{\{S\geq B\}}.}
$$

Indeed it is zero below $B$, equals $K-S$ between $B$ and $K$, and is zero above $K$. This supplies the terminal building block for reflection.

The zero-below-barrier property is a property of the terminal payoff. Before maturity, $F(S,t)$ need not vanish for $S<B$, because the ordinary European contracts can still finish above $B$. The killed [barrier option](../../../../../barrier-option.md) price, rather than this unrestricted European combination, is zero after a touch.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
