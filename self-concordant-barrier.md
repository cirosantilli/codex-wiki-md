# Self-concordant barrier

↑ **Parent:** [Interior-point method](interior-point-method.md)

A convex three-times differentiable barrier $F$ is self-concordant when

$$
|D^3F(x)[h,h,h]|\leq2\bigl(D^2F(x)[h,h]\bigr)^{3/2}.
$$

A barrier of parameter $\nu$ additionally satisfies $|DF(x)[h]|\leq\sqrt{\nu D^2F(x)[h,h]}$ and diverges at the domain boundary. Logarithmically homogeneous cone barriers satisfy $F(tx)=F(x)-\nu\log t$. The orthant barrier $-\sum_i\log x_i$ has parameter equal to the dimension, while the Lorentz-cone barrier $-\log(t^2-\|z\|^2)$ on $t>\|z\|$ has parameter two. Their Hessians define [Dikin ellipsoids](dikin-ellipsoid.md) and control interior Newton steps.

**Table of contents**

- [Logarithmically homogeneous barrier](logarithmically-homogeneous-barrier.md)
  - [Legendre dual cone barrier](legendre-dual-cone-barrier.md)
- [Dikin ellipsoid](dikin-ellipsoid.md)
- [Central path](central-path.md)
  - [Central-path Newton system](central-path-newton-system.md)

## ↑ Ancestors (7)

1. [Interior-point method](interior-point-method.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Dikin ellipsoid](dikin-ellipsoid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/4/a/solution.md)
- [Second-order cone programming](second-order-cone-programming.md)
