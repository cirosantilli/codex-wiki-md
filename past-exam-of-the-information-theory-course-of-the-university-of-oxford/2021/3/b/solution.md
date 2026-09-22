<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $T=g(Y)$. Because $T$ is determined by $Y$, the [chain rule for mutual information](../../../../chain-rule-for-mutual-information.md) gives

$$
I(X;Y)=I(X;Y,T)=I(X;T)+I(X;Y\mid T)\geq I(X;T).
$$

This is the [data processing inequality](../../../../data-processing-inequality.md). It holds for every input [probability distribution](../../../../probability-distribution-split.md). Maximizing each side over that same set of input [probability distributions](../../../../probability-distribution-split.md) gives **$C_{g(Y)}\leq C_Y$**; processing cannot increase [channel capacity](../../../../channel-capacity.md).

A simple sufficient condition for equality is that **$g$ be [injective](../../../../injective-function.md) on the reachable output [alphabet](../../../../alphabet.md)**. Then $Y$ can be recovered from $T$, giving $H(Y\mid T)=0$ and hence $I(X;Y\mid T)=0$ for every input law. The input that achieves the original [channel capacity](../../../../channel-capacity.md) therefore achieves it after processing as well. Values of $g$ outside reachable outputs are irrelevant.

[Injectivity](../../../../injective-function.md) is sufficient rather than necessary. More precisely, for [finite alphabets](../../../../finite-alphabet.md) [equality in capacity data processing](../../../../equality-in-capacity-data-processing.md) holds exactly when there is an original capacity-achieving input law for which $X$ and $Y$ have [conditional independence](../../../../conditional-independence.md) given $T$. Sufficiency follows from the displayed gap identity. For necessity, maximize $I(X;T)$ at an input law $p_*$; if its maximum equals $C_Y$, then $C_Y=I_{p_*}(X;T)\leq I_{p_*}(X;Y)\leq C_Y$, so both inequalities are equalities. Processing may discard output details unrelated to the input without losing [channel capacity](../../../../channel-capacity.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
