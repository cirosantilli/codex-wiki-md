# Lipschitz gradient

↑ **Parent:** [Gradient descent](gradient-descent-split.md)

A [differentiable function](differentiable-function.md) has a $\beta$-[Lipschitz gradient](lipschitz-gradient.md) on a set $D$ if its [gradient](gradient.md) satisfies [Lipschitz continuity](lipschitz-continuity.md) there:

$$
\|\nabla f(x)-\nabla f(y)\|_2\leq\beta\|x-y\|_2\qquad(x,y\in D),\quad \beta\geq0.
$$

All [norms](norm.md) here are the [Euclidean norm](euclidean-norm.md). The constant limits how fast the [gradient](gradient.md) changes; it is not a bound on the magnitude of the [gradient](gradient.md). For $f(x)=(x_1^2+9x_2^2)/2$, the [gradient](gradient.md) is the [linear map](linear-map.md) $x\mapsto\operatorname{diag}(1,9)x$. Its [operator norm](operator-norm.md) is $9$, so $\beta=9$ works globally and is sharp by taking $x-y=(0,1)^T$. The [gradient](gradient.md) itself is unbounded on the whole [Euclidean space](euclidean-norm.md).

If $f$ has a continuous [Hessian matrix](hessian-matrix.md) on an open [convex set](convex-set-split.md) $D$ and $\|\nabla^2f(z)\|_2\leq\beta$ throughout $D$, integrate that [linear map](linear-map.md) along the [line segment](line-segment.md) from $x$ to $y$:

$$
\nabla f(y)-\nabla f(x)=\int_0^1\nabla^2f(x+t(y-x))(y-x)\,dt.
$$

The [operator norm](operator-norm.md) bound proves the displayed [Lipschitz continuity](lipschitz-continuity.md). Convexity of the domain keeps the entire [line segment](line-segment.md) inside it. Bounding the [Hessian matrix](hessian-matrix.md) only at the endpoints is insufficient.

**Table of contents**

- [Descent lemma](descent-lemma.md)

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Baillon–Haddad theorem](baillon-haddad-theorem.md)
- [Descent lemma](descent-lemma.md)
- [Implicit nonsmooth block in alternating proximal-gradient iteration](implicit-nonsmooth-block-in-alternating-proximal-gradient-iteration.md)
- [Lipschitz gradient](lipschitz-gradient.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/2/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/7h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/1/e/solution.md)
- [Smooth maximum](smooth-maximum.md)
