<h1 id="18i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose first that $x$ is a [purely inseparable algebraic element](../../../../../../purely-inseparable-algebraic-element.md) over $K$, so

$$
x^{p^N}=y\in K
$$

for some $N\geq0$. Then $m_x$ divides $T^{p^N}-y$. Over an algebraic closure the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) is injective, so this polynomial has only one distinct root:

$$
T^{p^N}-y=(T-x)^{p^N}.
$$

Repeatedly use the zero-derivative criterion to write

$$
m_x(T)=q(T^{p^n})
$$

with $q'\ne0$. The polynomial $q$ is irreducible and therefore separable by part (a), but all its roots are powers of the single root $x$. Hence $q$ has degree one. Since $m_x$ is monic,

$$
m_x(T)=T^{p^n}-a
$$

for some $a\in K$.

Conversely, if the minimal polynomial has this form, then

$$
x^{p^n}=a\in K,
$$

so $x$ is purely inseparable. Thus the [minimal polynomial of a purely inseparable element](../../../../../../minimal-polynomial-of-a-purely-inseparable-element.md) is exactly

$$
\boxed{m_x(T)=T^{p^n}-a,\qquad n\geq0,\ a\in K.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18I](../../18i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
