<h1 id="20f/solution">Solution</h1>

↑ **Parent:** [20F](../20f.md)

The [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) states that for a number field of signature $(r_1,r_2)$,

$$
\mathcal O_K^\times\cong\mu(K)\times\mathbb Z^{r_1+r_2-1}.
$$

For $K=\mathbb Q(\sqrt5)$,

$$
\mathcal O_K=\mathbb Z[\phi],
\qquad \phi=\frac{1+\sqrt5}{2},
\qquad N(\phi)=-1.
$$

The field is real quadratic, so the unit rank is one and its only roots of unity are $\pm1$. To see that $\phi$ is fundamental, suppose a positive unit satisfies $1<u<\phi$. If its norm is $1$, its [integral](../../../../../integral.md) trace $u+u^{-1}$ lies strictly between $2$ and $\sqrt5$; if its norm is $-1$, its trace $u-u^{-1}$ lies strictly between $0$ and $1$. Neither interval contains an integer. Reducing any positive unit by a suitable power of $\phi$ now proves the [units of the quadratic field Q square root of five](../../../../../units-of-the-quadratic-field-q-square-root-of-five.md) formula

$$
\boxed{\mathcal O_K^\times=\{\mathord\pm\phi^n:n\in\mathbb Z\}}.
$$

If $\mathcal O_L^\times/\mathcal O_K^\times$ is finite, the two unit [groups](../../../../../group-split.md) have the same rank, namely one. Put $d=[L:K]$ and let $(r_1,r_2)$ be the signature of $L$. Then

$$
r_1+r_2-1=1,
\qquad
r_1+2r_2=[L:\mathbb Q]=2d.
$$

Therefore $r_1=4-2d$ and $r_2=2d-2$. For a proper extension, nonnegativity forces

$$
\boxed{d=2},
$$

with signature $(0,2)$.

This degree occurs: take $L=K(i)$. It is a totally imaginary quadratic extension of $K$, so the unit ranks agree and the quotient is finite. It is nontrivial because $i\in\mathcal O_L^\times$ but $i\notin\mathcal O_K^\times$ (and its coset has order two). This is the [finite relative unit quotient over a real quadratic field](../../../../../finite-relative-unit-quotient-over-a-real-quadratic-field.md) example.

## ↑ Ancestors (10)

1. [20F](../20f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
