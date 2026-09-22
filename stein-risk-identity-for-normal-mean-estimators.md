# Stein risk identity for normal mean estimators

↑ **Parent:** [Stein's lemma (probability)](stein-s-lemma-probability.md)

For $W\sim N_m(\eta,I)$, expand the squared estimation error and apply [Gaussian integration by parts](stein-s-lemma-probability.md) to each cross term. When $g$ satisfies the integrability and boundary conditions needed for that identity, this gives the displayed formula. For $g(w)=-a w/\|w\|^2$ and $m>2$, the origin singularity is integrable and the inner boundary term is $O(\varepsilon^{m-2})$, so the same identity applies by excision. Its divergence is $-a(m-2)/\|w\|^2$, giving risk $m+[a^2-2a(m-2)]\mathbb E\|W\|^{-2}$.

## ↑ Ancestors (8)

1. [Stein's lemma (probability)](stein-s-lemma-probability.md)
2. [Normal distribution](normal-distribution.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
