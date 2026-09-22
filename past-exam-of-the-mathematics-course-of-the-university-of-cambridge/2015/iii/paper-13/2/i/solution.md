<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take [information entropy](../../../../../../information-entropy.md) in bits and put $H(X_\varnothing)=0$. Write $C=A\cap B$, $U=A\setminus B$, and $V=B\setminus A$. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) gives

$$
\begin{aligned}
H(X_A)+H(X_B)-H(X_{A\cup B})-H(X_{A\cap B})
&=H(X_U\mid X_C)+H(X_V\mid X_C)-H(X_U,X_V\mid X_C)\\
&=H(X_U\mid X_C)-H(X_U\mid X_C,X_V)\\
&=I(X_U;X_V\mid X_C)\geq0.
\end{aligned}
$$

The last line uses nonnegativity of [conditional mutual information](../../../../../../conditional-mutual-information.md), equivalently the conditional version of [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md). All [random variables](../../../../../../random-variable-split.md) are finite-valued, so every [conditional entropy](../../../../../../conditional-entropy.md) here is finite. Therefore **the entropy [set function](../../../../../../set-function.md) is a [submodular set function](../../../../../../submodular-set-function.md)**:

$$
\boxed{H(X_A)+H(X_B)\geq H(X_{A\cup B})+H(X_{A\cap B}).}
$$

This is [entropy submodularity](../../../../../../entropy-submodularity.md), with equality precisely when $X_U$ and $X_V$ satisfy [conditional independence](../../../../../../conditional-independence.md) given $X_C$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
