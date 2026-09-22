<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $h$ in the [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md) $\mathcal H_k$, take the [directional derivative](../../../../../directional-derivative.md):

$$
\left.\frac d{d\epsilon}L(g+\epsilon h)\right|_{\epsilon=0}=\sum_i(g(x_i)-y_i)h(x_i).
$$

The [reproducing property](../../../../../reproducing-property.md) says $h(x_i)=\langle k(x_i,\cdot),h\rangle_{\mathcal H_k}$. Hence

$$
\left.\frac d{d\epsilon}L(g+\epsilon h)\right|_{\epsilon=0}=\left\langle\sum_i(g(x_i)-y_i)k(x_i,\cdot),h\right\rangle_{\mathcal H_k}.
$$

Each kernel section belongs to the [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md), so this finite sum is an admissible element. Uniqueness of a [vector](../../../../../vector.md) with these [inner products](../../../../../inner-product-split.md) gives the [functional gradient](../../../../../functional-gradient.md)

$$
\boxed{\nabla_gL(g)=\sum_{i=1}^n(g(x_i)-y_i)k(x_i,\cdot)}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
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
