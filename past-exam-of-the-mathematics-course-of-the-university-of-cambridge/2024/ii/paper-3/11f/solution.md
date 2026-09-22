<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The reduction map sends $H_k$ onto $H_{k-1}$ with kernel of order $p$, so $|H_k|=p^{k-1}$. More explicitly, the lifting-the-exponent calculation

$$
v_p((1+p)^{p^j}-1)=j+1
$$

shows that $1+p$ has order $p^{k-1}$ modulo $p^k$. Hence $H_k=\langle1+p\rangle$ is cyclic of that order.

For the [matrix](../../../../../matrix.md) claim, suppose $A\ne I$ and choose $m$ maximal such that $A=I+p^mB$, so some entry of $B$ is nonzero modulo $p$. Replacing $A$ by a suitable power, we may assume its order is a prime $q$. If $q\ne p$, binomial expansion modulo $p^{m+1}$ gives

$$
A^q\equiv I+qp^mB\not\equiv I\pmod {p^{m+1}}.
$$

If $q=p$, expansion modulo $p^{m+2}$ gives

$$
A^p\equiv I+p^{m+1}B\not\equiv I\pmod {p^{m+2}},
$$

because $p$ is odd. Both contradict $A^q=I$, so $A=I$.

For $p=2$, $r=1$ fails because $-I=I+2(-I)$ has order two. If $r=2$, the same argument works; in the order-two case, for maximal $m\geq2$,

$$
(I+2^mB)^2=I+2^{m+1}(B+2^{m-1}B^2)
e I,
$$

since the parenthesis is nonzero modulo two. Thus the smallest value is $r=2$.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
