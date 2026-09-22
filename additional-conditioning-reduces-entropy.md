# Additional conditioning reduces entropy

↑ **Parent:** [Conditioning reduces entropy](conditioning-reduces-entropy.md)

For finite [discrete random variables](discrete-random-variable.md) $X,Y,Z$, retaining $Y$ and also observing $Z$ gives

$$
H(X\mid Y)-H(X\mid Y,Z)=I(X;Z\mid Y)\geq0.
$$

Equality means [conditional independence](conditional-independence.md) of $X$ and $Z$ given $Y$. Both sides average over reports; the additional observation is retained alongside $Y$.[Definition 2.4 and Theorem 2.5(1), printed pp. 26–27](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

A short proof of the original inequality uses [Kullback-Leibler divergence](kullback-leibler-divergence.md):

$$
H(X)-H(X\mid Y)=I(X;Y)=\sum_{y:p_Y(y)>0}p_Y(y)D(p_{X\mid Y=y}\Vert p_X)\geq0.
$$

[Gibbs inequality](gibbs-inequality.md) makes each term nonnegative, vanishing exactly when $p_{X\mid Y=y}=p_X$: [independence](independent-random-variables.md) for every possible report. Applying this within each $Y=y$ and averaging proves the additional-conditioning inequality.[Theorem 2.1, printed p. 20; Theorem 2.3(1,3), printed p. 23; Theorem 2.4(2) and Corollary 2.4, printed p. 24](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

## ↑ Ancestors (7)

1. [Conditioning reduces entropy](conditioning-reduces-entropy.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
