# Soft-margin support vector machine

↑ **Parent:** [Support vector machine](support-vector-machine.md)

For signed training labels, a linear soft-margin [support vector machine](support-vector-machine.md) minimizes

$$
\frac12\lVert w\rVert^2+C\sum_i\xi_i,\qquad y_i(w^Tx_i+b)\geq1-\xi_i,\quad\xi_i\geq0,
$$

with $C>0$. Its [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) give $w=\sum_i\alpha_i y_ix_i$, $\sum_i\alpha_i y_i=0$, and $0\leq\alpha_i\leq C$.

**Table of contents**

- [Kernel support-vector coefficient from hinge activity](kernel-support-vector-coefficient-from-hinge-activity.md)
- [Support-vector leave-one-out error bound](support-vector-leave-one-out-error-bound.md)
- [Dual support vectors and margin degeneracy](dual-support-vectors-and-margin-degeneracy.md)

## ↑ Ancestors (9)

1. [Support vector machine](support-vector-machine.md)
2. [Classification in statistical learning](classification-in-statistical-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/2/c/solution.md)
