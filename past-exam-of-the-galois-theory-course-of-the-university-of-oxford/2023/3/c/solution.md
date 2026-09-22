<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $E=F(\alpha^p)\subseteq F(\alpha)$. If $\alpha$ is a [separable algebraic element](../../../../separable-algebraic-element.md) over $F$, its minimal polynomial over $E$ divides the original separable [minimal polynomial](../../../../minimal-polynomial.md). It also divides $T^p-\alpha^p=(T-\alpha)^p$, which has only one distinct root in any extension. Being separable with only one distinct root, that minimal polynomial has degree one. Hence $\alpha\in E$ and $F(\alpha)=F(\alpha^p)$.

Conversely, if the degree-$n$ minimal polynomial $m$ over $F$ is inseparable, part (b) writes it as $m(T)=g(T^p)$ with $\deg g=n/p$. Then $g(\alpha^p)=0$, so

$$
[F(\alpha^p):F]\leq n/p<n=[F(\alpha):F].
$$

The fields cannot be equal. This proves the equivalence

$$
\boxed{\alpha\text{ separable over }F\iff F(\alpha)=F(\alpha^p)},
$$

the [separability criterion using a pth power](../../../../separability-criterion-using-a-pth-power.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the galois theory course of the University of Oxford](../../../split.md)
5. [Galois theory course of the University of Oxford](../../../../galois-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
