<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiating the [gradient](../../../../../../gradient.md) term by term gives the [Hessian matrix](../../../../../../hessian-matrix.md)

$$
\nabla^2l(\mathbf x)=
\sum_{i=1}^n y_i f''(\mathbf a_i^{\mathsf T}\mathbf x)\,
\mathbf a_i\mathbf a_i^{\mathsf T}.
$$

Take row $i$ of $A$ to be $\mathbf a_i^{\mathsf T}$. Then

$$
\boxed{\nabla^2l=A^{\mathsf T}\Delta A,\qquad
\Delta_{ii}=y_i f''(\mathbf a_i^{\mathsf T}\mathbf x),\quad
\Delta_{ij}=0\ (i\ne j).}
$$

Indeed, entry $(j,k)$ of this product is $\sum_i\Delta_{ii}a_{ij}a_{ik}$, exactly the entry of the displayed sum of [outer products](../../../../../../outer-product.md). Explicitly,

$$
\Delta_{ii}=y_i\bigl((\mathbf a_i^{\mathsf T}\mathbf x)^2-1\bigr)
e^{-(\mathbf a_i^{\mathsf T}\mathbf x)^2/2}.
$$

These coefficients may have either sign, so a [positive-definite](../../../../../../positive-definite-bilinear-form.md) [Hessian matrix](../../../../../../hessian-matrix.md) cannot be assumed. This is an instance of the [Hessian of a sum of functions of linear forms](../../../../../../hessian-of-a-sum-of-functions-of-linear-forms.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
