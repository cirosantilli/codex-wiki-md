# Second-order Euler identity for homogeneous functions

↑ **Parent:** [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md)

Let $f$ be a twice continuously [differentiable function](differentiable-function.md) on an open domain stable under positive scaling, with $f(\lambda x)=\lambda^nf(x)$. Apply the [chain rule](chain-rule.md) twice to the scalar [function](function-split.md) $\lambda\mapsto f(\lambda x)$ and set $\lambda=1$. The result is

$$
\boxed{\sum_{i,j}x_ix_j\partial_i\partial_jf(x)=n(n-1)f(x).}
$$

In two variables, this reads $x^2f_{xx}+2xyf_{xy}+y^2f_{yy}=n(n-1)f$. In [matrix](matrix.md) notation it is $x^T(\nabla^2f)x=n(n-1)f$, where $\nabla^2f$ is the [Hessian matrix](hessian-matrix.md). Equivalently, the radial [differential operator](differential-operator.md) $D=\sum_ix_i\partial_i$ obeys $D^2f=Df+\sum_{i,j}x_ix_j\partial_i\partial_jf$; substituting $Df=nf$ explains the factor $n(n-1)$.

## ↑ Ancestors (7)

1. [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md)
2. [Homogeneous function](homogeneous-function.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/14/c/solution.md)
