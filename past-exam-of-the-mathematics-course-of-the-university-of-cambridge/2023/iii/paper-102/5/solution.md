<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For type $B_n$, the [spinor representation](../../../../../spin-representation.md) has highest weight

$$
\omega_n=\frac12(\varepsilon_1+\cdots+\varepsilon_n)
$$

and its weights are the $2^n$ sign vectors

$$
\frac12\sum_{j=1}^n i_j\varepsilon_j,\qquad i_j\in\{\pm1\}.
$$

Each weight has multiplicity one. Along the simple root $\alpha_j=\varepsilon_j-\varepsilon_{j+1}$, the [Kashiwara operator](../../../../../kashiwara-operator.md) $\widetilde e_j$ can raise a weight exactly when $(i_j,i_{j+1})=(-1,+1)$, when it replaces that pair by $(+1,-1)$. For the short root $\alpha_n=\varepsilon_n$, $\widetilde e_n$ replaces a final $-1$ by $+1$. This proves the stated crystal by the [root-string property of a crystal](../../../../../root-string-property-of-a-crystal.md).

For $n=3$, the complete list of raising edges is

$$
\begin{gathered}
(-,-,-)\xrightarrow{3}(-,-,+)
\xrightarrow{2}(-,+,-),\\
(-,+,-)\xrightarrow{1}(+,-,-),\qquad
(-,+,-)\xrightarrow{3}(-,+,+),\\
(+,-,-)\xrightarrow{3}(+,-,+),\qquad
(-,+,+)\xrightarrow{1}(+,-,+),\\
(+,-,+)\xrightarrow{2}(+,+,-)
\xrightarrow{3}(+,+,+).
\end{gathered}
$$

The [tensor product of crystals](../../../../../tensor-product-of-crystals.md) has four highest-weight connected components, of highest weights

$$
0,\qquad\omega_1,\qquad\omega_2,\qquad2\omega_3.
$$

Consequently, for the eight-dimensional spin representation $S$ of $\mathfrak{so}_7$,

$$
S\otimes S
\cong
\mathbb C\oplus V(\omega_1)\oplus V(\omega_2)\oplus V(2\omega_3),
$$

with dimensions

$$
64=1+7+21+35.
$$

Equivalently these summands are $\Lambda^k(\mathbb C^7)$ for $0\leq k\leq3$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
