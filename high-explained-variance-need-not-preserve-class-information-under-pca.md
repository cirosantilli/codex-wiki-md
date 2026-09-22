# High explained variance need not preserve class information under PCA

↑ **Parent:** [Principal component analysis](principal-component-analysis.md)

Let $W,S$ be independent balanced variables with values $-1,1$, and let $X=(aW,bS)^T$ with $a>b>0$ and class $Y=S$. Then $E[X]=0$ and $\operatorname{Cov}(X)=\operatorname{diag}(a^2,b^2)$. The first [principal component](principal-component.md) is the first coordinate and explains $a^2/(a^2+b^2)$ of total [variance](variance-split.md). Yet it is independent of $Y$, so even the best [classifier](classifier.md) using only that coordinate has accuracy $1/2$. The second coordinate determines $Y$ exactly. Taking $a/b$ arbitrarily large makes the retained [variance](variance-split.md) approach one without improving class accuracy. Adding a constant baseline to each coordinate preserves the centered result and permits positive neural rates.

## ↑ Ancestors (8)

1. [Principal component analysis](principal-component-analysis.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
