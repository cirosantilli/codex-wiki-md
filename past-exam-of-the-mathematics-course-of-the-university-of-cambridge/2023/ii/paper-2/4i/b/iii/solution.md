<h1 id="4i/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $A=\operatorname{ran}f$ for a [partial computable function](../../../../../../../computable-function.md) $f$. Since $A\ne\varnothing$, fix $a_0\in A$. Decode each input $w$ as a pair $((w)_0,(w)_1)=(u,t)$. Using the [truncated computation function](../../../../../../../truncated-computation-function.md), define

$$
h(w)=
\begin{cases}
f(u),&\text{if the computation of $f(u)$ halts within $t$ steps},\\
a_0,&\text{otherwise}.
\end{cases}
$$

This is a [total computable function](../../../../../../../total-computable-function.md), and every output lies in $A$. Conversely, if $a=f(u)$, choosing $t$ at least the halting time gives an input $w$ with $h(w)=a$. Thus $\operatorname{ran}h=A$, proving (iii)$\Rightarrow$(iv).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4I](../../../4i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
