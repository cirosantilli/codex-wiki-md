<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The maximizer defining $g^*(x)$ is $\operatorname{prox}_{tf}(x)$, so

$$
\boxed{\nabla M_tf(x)=\frac1t[x-\operatorname{prox}_{tf}(x)].}
$$

Consequently

$$
x_{k+1}=\operatorname{prox}_{tf}(x_k)
=x_k-t\nabla M_tf(x_k).
$$

**Thus the [proximal point algorithm](../../../../../../../proximal-point-algorithm.md) for $f$ is ordinary [gradient descent](../../../../../../../gradient-descent.md) with step $t$ on its smooth Moreau envelope.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
