<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\Diamond'_S$ for the countable-family assertion in the PDF; its prime is not a superscript $c$. A single [stationary diamond at a regular cardinal](../../../../../../stationary-diamond-at-a-regular-cardinal.md) sequence gives such families by taking singletons, so $\Diamond_S\Rightarrow\Diamond'_S$.

Conversely enumerate each countable family as $E_\alpha(n)$, $n<\omega$, padding finite families and allowing the empty set as a default. Fix a [bijection](../../../../../../bijection.md) $\pi:\lambda\times\omega\to\lambda$. The previous part applied to $B(\xi)=\{\pi(\xi,n):n<\omega\}$ gives a [club set](../../../../../../club-set.md) $D$ on which $\pi[\alpha\times\omega]\subseteq\alpha$. Define, for each $n$, a single candidate sequence

$$
D^n_\alpha=\{\xi<\alpha:\pi(\xi,n)\in E_\alpha(n)\}\qquad(\alpha\in S).
$$

Suppose no candidate sequence witnesses $\Diamond_S$. For each $n$ choose $X_n\subseteq\lambda$ and a [club set](../../../../../../club-set.md) $C_n$ such that $D^n_\alpha\ne X_n\cap\alpha$ for every $\alpha\in S\cap C_n$. Code all the counterexamples into

$$
X=\{\pi(\xi,n):n<\omega,\ \xi\in X_n\}.
$$

The countable-family hypothesis guesses $X$ on a stationary set. Choose a guessing $\alpha$ in the [club set](../../../../../../club-set.md) $D\cap\bigcap_n C_n$, and choose $n$ with $E_\alpha(n)=X\cap\alpha$. For every $\xi<\alpha$, closure under $\pi$ gives

$$
\xi\in D^n_\alpha\ \Longleftrightarrow\ \pi(\xi,n)\in X
\ \Longleftrightarrow\ \xi\in X_n.
$$

Thus $D^n_\alpha=X_n\cap\alpha$, contradicting $\alpha\in C_n$. At least one candidate is a diamond sequence, proving

$$
\boxed{\Diamond'_S\ \Longleftrightarrow\ \Diamond_S.}
$$

This is the [countable-family diamond equivalence](../../../../../../countable-family-diamond-equivalence.md), for every regular uncountable $\lambda$ and stationary $S\subseteq\lambda$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
