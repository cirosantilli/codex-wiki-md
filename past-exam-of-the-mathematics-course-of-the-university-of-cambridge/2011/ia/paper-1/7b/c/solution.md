<h1 id="7b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [eigenvector](../../../../../../eigenvector.md) [basis](../../../../../../basis.md) $v_1=(-1,0,1)^T$, $v_2=(1,1,0)^T$, $v_3=(1,1,1)^T$. The forcing has decomposition $b=-v_1+3v_3$. If $x=c_1v_1+c_2v_2+c_3v_3$, the [linear system](../../../../../../system-of-linear-equations.md) reduces to

$$
(1-\lambda)c_1=-1,\qquad(2-\lambda)c_2=0,\qquad(3-\lambda)c_3=3.
$$

For $\lambda=0$, all coefficients are determined, giving

$$
\boxed{x=(2,1,0)^T.}
$$

For $\lambda=1$, the first equation would say $0=-1$, so **there are no solutions**. For $\lambda=2$, $c_1=1$, $c_3=3$, and $c_2$ is arbitrary. Thus **all solutions** are

$$
\boxed{x=(2,3,4)^T+t(1,1,0)^T,\qquad t\in\mathbb R.}
$$

These outcomes illustrate respectively an invertible [matrix](../../../../../../matrix.md), incompatible forcing outside its [image of a linear map](../../../../../../image-of-a-linear-map.md), and a compatible forcing with a nontrivial [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
