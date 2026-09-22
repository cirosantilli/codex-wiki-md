<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $h=h^*$. The exponential $u_t=e^{ith}$ is defined by its norm-convergent power series. Continuity and conjugate linearity of the [involution](../../../../../../involution.md) give $u_t^*=e^{-ith}$, and multiplication of the commuting exponential series gives $u_t^*u_t=u_tu_t^*=1$. Thus $u_t$ is a [Unitary element of a C-star algebra](../../../../../../unitary-element-of-a-c-star-algebra.md) and, by the [C-star identity](../../../../../../c-star-identity.md), $\|u_t\|=1$.

A [character of an algebra](../../../../../../character-of-an-algebra.md) is automatically continuous with $|\varphi(a)|\le\|a\|$, as proved in Question 5. Passing it through the exponential series gives

$$
|e^{it\varphi(h)}|=|\varphi(u_t)|\le1\qquad(t\in\mathbb R).
$$

The left side is $e^{-t\Im\varphi(h)}$. Considering both signs of $t$ forces $\Im\varphi(h)=0$. So characters take real values on [self-adjoint C-star elements](../../../../../../hermitian-element-of-a-c-star-algebra.md).

Now write $x=h+ik$ with

$$
h=\frac{x+x^*}{2},\qquad k=\frac{x-x^*}{2i},
$$

both [self-adjoint C-star elements](../../../../../../hermitian-element-of-a-c-star-algebra.md). Then

$$
\boxed{\varphi(x^*)=\varphi(h)-i\varphi(k)=\overline{\varphi(h)+i\varphi(k)}=\overline{\varphi(x)}.}
$$

This proves that [characters of a C-star algebra respect the involution](../../../../../../characters-of-a-c-star-algebra-respect-the-involution.md). The argument itself does not require commutativity, although a noncommutative algebra need not have any characters.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
