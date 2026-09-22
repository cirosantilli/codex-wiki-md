# Delta rule

↑ **Parent:** [Error-correction learning](error-correction-learning.md)

For a linear output $y=Wx$ and squared loss $L=\|t-y\|^2/2$, [gradient descent](gradient-descent-split.md) gives $\Delta W=\eta(t-y)x^{\mathsf T}$. Indeed $\partial L/\partial W_{ij}=-(t_i-y_i)x_j$. On the same example, $e'=(1-\eta\|x\|^2)e$, proving strict error reduction when $e\ne0$ and $0<\eta\|x\|^2<2$.

## ↑ Ancestors (9)

1. [Error-correction learning](error-correction-learning.md)
2. [Supervised learning](supervised-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cerebellar error-driven learning](cerebellar-error-driven-learning.md)
- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/5/solution.md)
