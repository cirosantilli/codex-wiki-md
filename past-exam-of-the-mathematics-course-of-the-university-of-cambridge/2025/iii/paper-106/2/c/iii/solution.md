<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Start with the sequence from part ii. For each $n$, the definition of the [operator norm](../../../../../../../operator-norm.md) gives $x_n\in B_X$ with

$$
|(g_n-f)(x_n)|>\varepsilon/2.
$$

Because $g_n\xrightarrow{w^*}f$, pass recursively to a subsequence so far out that its $n$th member also satisfies

$$
|(g_n-f)(x_m)|<\varepsilon/4
\qquad(m<n).
$$

Part b supplies a weakly Cauchy subsequence $(x_{k_j})$. Put

$$
y_j=\frac{x_{k_{2j}}-x_{k_{2j-1}}}{2}\in B_X,
\qquad
h_j=g_{k_{2j}}.
$$

Then $(y_j)$ is weakly null, $h_j\xrightarrow{w^*}f$, and the two preceding estimates give

$$
|(h_j-f)(y_j)|
\geq\frac12\left(|(h_j-f)(x_{k_{2j}})|-|(h_j-f)(x_{k_{2j-1}})|\right)
>\varepsilon/8.
$$

Since $f(y_j)\to0$, discard finitely many terms to obtain $|h_j(y_j)|>\varepsilon/16$ for every remaining $j$. Relabelling proves the claim.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 106](../../../../paper-106-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
