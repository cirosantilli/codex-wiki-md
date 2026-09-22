<h1 id="25i/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use angular coordinate $v$. The two surfaces have parametrizations

$$
R(u,v)=(e^u\cos v,e^u\sin v,u),
$$

and

$$
S(s,v)=(\cosh s\cos v,\cosh s\sin v,s).
$$

The supplied surface-of-revolution formula gives

$$
K_R(u)=-\frac1{(1+e^{2u})^2},
\qquad
K_S(s)=-\frac1{\cosh^4s}.
$$

Since $s>0$, the change of coordinate

$$
u=\log(\sinh s)
$$

is a diffeomorphism from $(0,\infty)$ to $\mathbb R$ and satisfies $1+e^{2u}=\cosh^2s$. Therefore

$$
\boxed{
\phi(S(s,v))=R(\log(\sinh s),v)
}
$$

is a diffeomorphism and obeys $K_R\circ\phi=K_S$. This is the [curvature-matching diffeomorphism between two surfaces of revolution](../../../../../../../curvature-matching-diffeomorphism-between-two-surfaces-of-revolution.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [25I](../../../25i.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
