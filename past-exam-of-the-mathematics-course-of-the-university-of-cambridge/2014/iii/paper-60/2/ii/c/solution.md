<h1 id="2/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $Z$ is determined by $X,Y$, its [conditional entropy](../../../../../../../conditional-entropy.md) satisfies $H(Z\mid X,Y)=0$. Equate the two forms of the [chain rule for conditional entropy](../../../../../../../chain-rule-for-conditional-entropy.md) to obtain

$$
H(X\mid Y)=H(Z\mid Y)+H(X\mid Z,Y).
$$

Conditioning cannot increase classical [Shannon entropy](../../../../../../../information-entropy.md): $H(Z)-H(Z\mid Y)=I(Z:Y)\geq0$ by nonnegativity of [mutual information](../../../../../../../mutual-information.md). Thus $H(Z\mid Y)\leq H(Z)=h(p_e)$. When $Z=0$, the value of $X$ is exactly $f(Y)$ and $H(X\mid Y,Z=0)=0$. When $Z=1$ and $Y=y$, the value $f(y)$ is excluded, leaving at most $|J_X|-1$ possibilities. By [maximum entropy on a finite alphabet](../../../../../../../maximum-entropy-on-a-finite-alphabet.md),

$$
H(X\mid Y,Z=1)\leq\log_2(|J_X|-1).
$$

Averaging the two conditional cases now yields

$$
H(X\mid Z,Y)\leq p_e\log_2(|J_X|-1),
$$

and consequently

$$
\boxed{H(X\mid Y)\leq h(p_e)+p_e\log_2(|J_X|-1).}
$$

This is [Fano's inequality via an error indicator](../../../../../../../fano-s-inequality-via-an-error-indicator.md). Events of zero probability contribute zero to the average and need no conditional distribution. For $|J_X|=1$, the inference is automatically correct and the entropy is zero; the displayed logarithmic form is intended for $|J_X|\geq2$. Optimality of the guess is not needed for the inequality: it holds for every deterministic $f$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 60](../../../../paper-60-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
