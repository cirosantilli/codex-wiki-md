<h1 id="3/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $t>0$, [positive homogeneity](../../../../../../../positively-homogeneous-function-degree-one.md) and [concavity](../../../../../../../concave-function.md) give

$$
\begin{aligned}
f(X+tY)
&=(1+t)f\left(\frac{X}{1+t}+\frac{tY}{1+t}\right)\\
&\geq(1+t)\left(\frac1{1+t}f(X)+\frac t{1+t}f(Y)\right)\\
&=f(X)+tf(Y).
\end{aligned}
$$

After subtracting $f(X)$, dividing by $t$, and taking the one-sided [directional derivative](../../../../../../../directional-derivative.md) at zero,

$$
\boxed{\left.\frac d{dt}\right|_{t=0^+}f(X+tY)\geq f(Y)}.
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
