<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and define the positive [self-adjoint operator](../../../../../../self-adjoint-operator.md)

$$
B=(1-\partial_x^2)^{1/2}
$$

on $L^2(\mathbb T)$. On the Fourier mode $e^{inx}$ it acts by multiplication by $\sqrt{1+n^2}$. Consequently

$$
D(B)=H^1(\mathbb T),
\qquad
D(B^2)=H^2(\mathbb T).
$$

The energy space is the [periodic Sobolev space](../../../../../../periodic-sobolev-space.md)

$$
\boxed{\mathcal H=H^1(\mathbb T)\times L^2(\mathbb T)},
$$

with inner product

$$
((u,v),(p,q))_{\mathcal H}
=(Bu,Bp)_{L^2}+(v,q)_{L^2}.
$$

If $u=\sum u_ne^{inx}$ and $v=\sum v_ne^{inx}$, then

$$
\|(u,v)\|_{\mathcal H}^2
=2\pi\sum_{n\in\mathbb Z}
[(1+n^2)|u_n|^2+|v_n|^2],
$$

which is precisely the stated energy norm.

With $v=u_t$, the periodic [Klein-Gordon equation](../../../../../../klein-gordon-equation.md) becomes

$$
\dot Z=AZ,
\qquad
A=\begin{pmatrix}0&I\\-B^2&0\end{pmatrix},
\qquad
A(u,v)=(v,-B^2u).
$$

For $AZ$ to belong to $H^1\times L^2$, one needs $v\in H^1$ and $u\in H^2$. Thus

$$
\boxed{D(A)=H^2(\mathbb T)\times H^1(\mathbb T)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
