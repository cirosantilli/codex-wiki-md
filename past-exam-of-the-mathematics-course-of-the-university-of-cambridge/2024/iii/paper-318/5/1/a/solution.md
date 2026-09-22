<h1 id="5/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose first that $f-u^*$ is [orthogonal](../../../../../../../orthogonal-vectors.md) to $\mathcal U_n$. Every $u\in\mathcal U_n$ can be written $u=u^*+v$ with $v\in\mathcal U_n$. The [Pythagorean theorem in an inner-product space](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|f-u\|^2
=\|(f-u^*)-v\|^2
=\|f-u^*\|^2+\|v\|^2
\geq\|f-u^*\|^2.
$$

Thus $u^*$ is a best approximation.

Conversely, if $u^*$ minimizes the distance, then for every $v\in\mathcal U_n$ the quadratic

$$
q(t)=\|f-u^*-tv\|^2
$$

has its minimum at $t=0$. Differentiating there gives $q'(0)=-2(f-u^*,v)=0$ in the real case; varying real and imaginary parts gives the complex case. Therefore

$$
\boxed{u^*\text{ is best}
\iff(f-u^*,v)=0\quad\forall v\in\mathcal U_n}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [5](../../../5.md)
4. [Paper 318](../../../../paper-318-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
