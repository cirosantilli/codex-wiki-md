<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\pi_n=\zeta_{p^n}-1$. The shifted cyclotomic polynomial

$$
\Phi_{p^n}(1+X)
=\frac{(1+X)^{p^n}-1}{(1+X)^{p^{n-1}}-1}
$$

is Eisenstein at $p$. Therefore it is irreducible, $\pi_n$ is a uniformizer, and

$$
[\mathbb Q_p(\zeta_{p^n}):\mathbb Q_p]
=\varphi(p^n)=p^{n-1}(p-1),
$$

so the extension is totally ramified. It is the splitting field of $\Phi_{p^n}$, and every automorphism is uniquely

$$
\zeta_{p^n}\longmapsto\zeta_{p^n}^{,a},
\qquad a\in(\mathbb Z/p^n\mathbb Z)^\times.
$$

This proves the [cyclotomic extension of a p-adic field](../../../../../../cyclotomic-extension-of-a-p-adic-field.md) isomorphism

$$
\operatorname{Gal}(\mathbb Q_p(\zeta_{p^n})/\mathbb Q_p)
\cong(\mathbb Z/p^n\mathbb Z)^\times.
$$

Restriction in the cyclotomic tower corresponds to reduction of $a$, so taking the [inverse limit](../../../../../../inverse-limit.md) gives

$$
\boxed{\operatorname{Gal}(\mathbb Q_p(\zeta_{p^\infty})/\mathbb Q_p)
\cong\varprojlim_n(\mathbb Z/p^n\mathbb Z)^\times
=\mathbb Z_p^\times.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
