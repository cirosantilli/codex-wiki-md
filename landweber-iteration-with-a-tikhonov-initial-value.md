# Landweber iteration with a Tikhonov initial value

↑ **Parent:** [Landweber iteration](landweber-iteration.md)

Initialize [Landweber iteration](landweber-iteration.md) by [Tikhonov regularization](tikhonov-regularization.md), then use step $1/\alpha$. Writing $B=A^*A$ and $R=I-B/\alpha$, the iterate is $x_n=R^n(B+\alpha I)^{-1}A^*y+\alpha^{-1}\sum_{j=0}^{n-1}R^jA^*y$. For nonzero $A$, the sufficient convergence condition is $\alpha>\|A\|^2/2$. This explicit method differs from [Iterated Tikhonov regularization](iterated-tikhonov-regularization.md), whose update is $(B+\alpha I)x_{n+1}=\alpha x_n+A^*y$.

**Table of contents**

- [Closed form of a Tikhonov-initialized Landweber iterate](closed-form-of-a-tikhonov-initialized-landweber-iterate.md)

## ↑ Ancestors (7)

1. [Landweber iteration](landweber-iteration.md)
2. [Normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Closed form of a Tikhonov-initialized Landweber iterate](closed-form-of-a-tikhonov-initialized-landweber-iterate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/3/c/solution.md)
