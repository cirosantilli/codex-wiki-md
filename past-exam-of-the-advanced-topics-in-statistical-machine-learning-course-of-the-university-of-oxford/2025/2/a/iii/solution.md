<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [closure property of positive-semidefinite kernels](../../../../../closure-property-of-positive-semidefinite-kernels.md) gives three constructions, each seen directly from the [feature maps](../../../../../feature-map.md) $\varphi_1,\varphi_2$.

- **Nonnegative sums:** $k=\alpha k_1+\beta k_2$, for $\alpha,\beta\geq0$. Its [feature map](../../../../../feature-map.md) is $(\sqrt\alpha\varphi_1(x),\sqrt\beta\varphi_2(x))$ in the [Hilbert space](../../../../../hilbert-space-split.md) direct sum; expanding its [inner product](../../../../../inner-product-split.md) gives $k$.
- **Pointwise products:** $k(x,x')=k_1(x,x')k_2(x,x')$. In the Hilbert [tensor product](../../../../../tensor-product.md), use $\varphi(x)=\varphi_1(x)\otimes\varphi_2(x)$: the [inner product](../../../../../inner-product-split.md) of two such elementary tensors is the product of their two [inner products](../../../../../inner-product-split.md).
- **Input-dependent weighting:** $k(x,x')=a(x)k_1(x,x')a(x')$ for any real-valued function $a$. Its [feature map](../../../../../feature-map.md) is $a(x)\varphi_1(x)$, so signs of $a$ are allowed. Nonnegative scalar multiplication is the special case of constant $a$; the weighting factor $a(x)a(x')$ is itself a rank-one [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel-split.md).

Another useful consequence is pullback: if $h:\mathcal X\to\mathcal Z$ and $k_0$ is a [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel-split.md) on $\mathcal Z$, then $k_0(h(x),h(x'))$ has [feature map](../../../../../feature-map.md) $\varphi_0\circ h$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
