<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $c=1/(a-1)$. If $X_0=x>c$, then for either possible sign,

$$
X_{n+1}\geq aX_n-1,\qquad
X_{n+1}-X_n\geq(a-1)X_n-1>0
$$

as long as $X_n>c$. Thus the process stays above $c$, is strictly increasing, and induction gives $X_n\geq c+a^n(x-c)\to\infty$. If $x<-c$, the symmetric argument makes the process strictly decreasing to $-\infty$. This proves the first assertion pathwise, with the strict sufficient threshold $|x|>c$.

For an arbitrary starting point, a proof is needed that the process actually reaches such a region. Fix $L>c$ and choose an integer $m$ so

$$
\sum_{j=0}^{m-1}a^j=\frac{a^m-1}{a-1}>L.
$$

At a block starting at time $km$, if $X_{km}\geq0$, the next $m$ signs all equal to $+1$ give $X_{(k+1)m}>L$. If $X_{km}<0$, all $-1$ signs instead give $X_{(k+1)m}<-L$. Conditional on the current [natural filtration](../../../../../../natural-filtration.md), the selected block has probability $\varepsilon=2^{-m}$, by [independence](../../../../../../independent-random-variables.md) of future signs. If $\tau=\inf\{n:|X_n|>L\}$, iterated [conditional expectation](../../../../../../conditional-expectation.md) gives

$$
\mathbb P_x(\tau>km)\leq(1-\varepsilon)^k\longrightarrow0.
$$

This is a [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md), so $\tau<\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Once outside, the sign is preserved and, for every future noise sequence,

$$
|X_{\tau+j}|\geq c+a^j(|X_\tau|-c)\longrightarrow\infty.
$$

Consequently the [explosive affine recursion with symmetric bounded noise](../../../../../../explosive-affine-recursion-with-symmetric-bounded-noise.md) has

$$
\boxed{\mathbb P_x\!\left(\lim_{n\to\infty}|X_n|=\infty\right)=1\quad\text{for every }x\in\mathbb R.}
$$

The block argument closes the gap between escape from a large initial value and escape from an arbitrary one; no assertion about the absence of atoms in an infinite random series is necessary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
