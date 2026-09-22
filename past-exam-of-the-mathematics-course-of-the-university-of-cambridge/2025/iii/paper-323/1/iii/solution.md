<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $p=(d+1)/(2d)$, the weighted difference of the two [Werner–Holevo channels](../../../../../../werner-holevo-channel.md) is

$$
\begin{aligned}
\bigl(pT_+-(1-p)T_-\bigr)(X)
&=\frac1{2d}\bigl(\operatorname{Tr}(X)I+X^T\bigr)
-\frac1{2d}\bigl(\operatorname{Tr}(X)I-X^T\bigr)\\
&=\frac1dX^T.
\end{aligned}
$$

Thus the map is the [transposition map](../../../../../../transpose.md) divided by $d$. The [diamond norm of the transposition map](../../../../../../diamond-norm-of-the-transposition-map.md) and invariance of the [trace norm](../../../../../../trace-norm.md) under [matrix transpose](../../../../../../transpose.md) give

$$
\boxed{\|pT_+-(1-p)T_-\|_\diamond
=\frac1d\|\Theta\|_\diamond=1},
\qquad
\boxed{\|pT_+-(1-p)T_-\|_1
=\frac1d\|\Theta\|_1=\frac1d}.
$$

Substitution into the optimal-error formulas shows that an entangled [quantum ancilla](../../../../../../quantum-ancilla.md) permits perfect discrimination, whereas every ancilla-free strategy has

$$
\boxed{P_{\mathrm{err}}^{\mathrm{no\ anc}}=\frac12\left(1-\frac1d\right)}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
