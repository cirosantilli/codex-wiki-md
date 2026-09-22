# Bias and variance of a three-neighbour weighted smoother

↑ **Parent:** [K-nearest neighbors algorithm](k-nearest-neighbors-algorithm.md)

With fixed neighbor positions, independent equal-variance errors and weights $w,(1-w)/2,(1-w)/2$, the displayed [variance](variance-split.md) is minimized at $w=1/3$, with value $\sigma^2/3$. Its [bias](bias-of-an-estimator.md) is $w m_1+(1-w)(m_2+m_3)/2-m(x)$. Larger nearest-point weight often reduces smoothing bias, but neither the bias nor the variance is universally monotone over $0<w<1$. If the nearest point is the target, the squared bias is $(1-w)^2[(m_2+m_3)/2-m(x)]^2$.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (9)

1. [K-nearest neighbors algorithm](k-nearest-neighbors-algorithm.md)
2. [Classification in statistical learning](classification-in-statistical-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/1/c/solution.md)
