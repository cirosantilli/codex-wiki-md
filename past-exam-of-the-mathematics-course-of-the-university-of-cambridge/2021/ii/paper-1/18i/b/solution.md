<h1 id="18i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The seventh [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) is

$$
\Phi_7(X)=X^6+X^5+X^4+X^3+X^2+X+1.
$$

It is irreducible over $\mathbb Q$, and all its roots $\zeta_7^a$, $a=1,\ldots,6$, lie in $L=\mathbb Q(\zeta_7)$. Hence $L/\mathbb Q$ is a degree-six [Finite Galois extension](../../../../../../finite-galois-extension.md), with

$$
G=\operatorname{Gal}(L/\mathbb Q)
=\{\sigma_a:a\in(\mathbb Z/7\mathbb Z)^\times\},
\qquad
\sigma_a(\zeta_7)=\zeta_7^a.
$$

The group $(\mathbb Z/7\mathbb Z)^\times$ is cyclic of order six; for example,

$$
G=\langle\sigma_3\rangle\cong C_6.
$$

By the [Galois correspondence](../../../../../../galois-correspondence.md), the subfields are the fixed fields of the four subgroups of $C_6$:

$$
\begin{array}{c|c|c}
\operatorname{Gal}(L/M)&[M:\mathbb Q]&M\\ \hline
G&1&\mathbb Q\\
\{\sigma_1,\sigma_2,\sigma_4\}&2&
\mathbb Q(\eta),\quad
\eta=\zeta_7+\zeta_7^2+\zeta_7^4\\
\{\sigma_1,\sigma_6\}&3&
\mathbb Q(\theta),\quad
\theta=\zeta_7+\zeta_7^{-1}\\
\{\sigma_1\}&6&L.
\end{array}
$$

Thus these are all the subfields.

For the [Quadratic Gaussian period in the seventh cyclotomic field](../../../../../../quadratic-gaussian-period-in-the-seventh-cyclotomic-field.md), put

$$
\bar\eta=\zeta_7^3+\zeta_7^5+\zeta_7^6.
$$

The cyclotomic relation gives $\eta+\bar\eta=-1$, while direct multiplication gives $\eta\bar\eta=2$. Hence

$$
\eta^2+\eta+2=0.
$$

Its discriminant is $-7$, so

$$
\eta=\frac{-1+\sqrt{-7}}2,
\qquad
m_{\eta,\mathbb Q}(X)=X^2+X+2.
$$

For the [real cubic subfield of the seventh cyclotomic field](../../../../../../real-cubic-subfield-of-the-seventh-cyclotomic-field.md), divide

$$
1+\zeta_7+\cdots+\zeta_7^6=0
$$

by $\zeta_7^3$. With $\theta=\zeta_7+\zeta_7^{-1}$,

$$
\zeta_7^2+\zeta_7^{-2}=\theta^2-2,
\qquad
\zeta_7^3+\zeta_7^{-3}=\theta^3-3\theta,
$$

so

$$
\theta^3+\theta^2-2\theta-1=0.
$$

This cubic has no rational root, and therefore

$$
m_{\theta,\mathbb Q}(X)=X^3+X^2-2X-1.
$$

The requested [primitive elements](../../../../../../primitive-element-of-a-field-extension.md), [minimal polynomials](../../../../../../minimal-polynomial-of-an-algebraic-element.md), and automorphism groups are consequently

$$
\begin{array}{c|c|c|c|c}
M&\text{primitive element}&m(X)&\operatorname{Aut}(M/\mathbb Q)&
\operatorname{Aut}(L/M)\\ \hline
\mathbb Q&0&X&1&C_6\\
\mathbb Q(\eta)&\eta&X^2+X+2&C_2&
\{\sigma_1,\sigma_2,\sigma_4\}\cong C_3\\
\mathbb Q(\theta)&\theta&X^3+X^2-2X-1&C_3&
\{\sigma_1,\sigma_6\}\cong C_2\\
L&\zeta_7&\Phi_7(X)&C_6&1.
\end{array}
$$

More explicitly, the nontrivial automorphism of $\mathbb Q(\eta)$ sends

$$
\eta\longmapsto\bar\eta=-1-\eta,
$$

and the three automorphisms of $\mathbb Q(\theta)$ cyclically permute

$$
\zeta_7+\zeta_7^{-1},\qquad
\zeta_7^2+\zeta_7^{-2},\qquad
\zeta_7^4+\zeta_7^{-4}.
$$

Finally, $G$ is abelian, so every subgroup is normal. The [subextensions of an abelian Galois extension](../../../../../../subextensions-of-an-abelian-galois-extension.md) theorem shows that

$$
\boxed{\text{all four subfields }M\text{ are Galois over }\mathbb Q}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18I](../../18i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
