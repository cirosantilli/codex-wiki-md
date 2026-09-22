<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $X=1+T$ and let $\varphi$ be the [Frobenius substitution on cyclotomic power series](../../../../../../frobenius-substitution-on-cyclotomic-power-series.md), $\varphi(g)(T)=g(X^p-1)$. It is injective: modulo $p$ it is the injective map $\overline g(T)\mapsto\overline g(T^p)$. If $\varphi(g)=0$, this makes every coefficient of $g$ divisible by $p$; dividing by $p$ and repeating makes every coefficient zero.

We prove that $R$ is a [finite free module](../../../../../../finite-free-module.md) over $S=\varphi(R)$ of rank $p$, with basis $1,X,\ldots,X^{p-1}$. Modulo $p$, every series has a unique decomposition over $\mathbb F_p[[T^p]]$ in the basis $1,T,\ldots,T^{p-1}$. Changing to the powers of $X=1+T$ is an invertible triangular change of basis. Thus, modulo $p$, every $h\in R$ can be expressed as $\sum_{i=0}^{p-1}X^i\varphi(h_i)$. Lift the coefficients to $R$, subtract this expression, and divide the remainder by $p$. Repeating and summing the p-adically convergent coefficient series gives

$$
h=\sum_{i=0}^{p-1}X^i\varphi(h_i),\qquad h_i\in R.
$$

Uniqueness follows by reduction modulo $p$ and successive division by $p$. This proves finite freeness, not just a formal invariance of the right side in the question.

For $f\in R^\times$, multiplication by $f$ is an invertible $S$-linear map $m_f:R\to R$. Its [determinant](../../../../../../determinant.md) $b=\det_S(m_f)$ belongs to $S^\times$. Define

$$
\boxed{Nf=\varphi^{-1}\bigl(\det_S(m_f)\bigr).}
$$

This is the [norm for a finite free ring extension](../../../../../../norm-for-a-finite-free-ring-extension.md), pulled back along the injective substitution, and it is multiplicative and unit-valued.

To identify its [determinant](../../../../../../determinant.md) with the desired product, extend coefficients to $\mathcal O=\mathbb Z_p[\mu_p]$. The substitutions $X\mapsto\xi X$ for $\xi^p=1$ are continuous automorphisms of $\mathcal O[[T]]$ fixing $\varphi(\mathcal O[[T]])$. Evaluation of a series at $\xi X-1$ is legitimate in the $(\xi-1,T)$-adic topology, because the constant term $\xi-1$ is topologically nilpotent. On fraction [fields](../../../../../../field.md) this is a degree-$p$ extension with these $p$ distinct automorphisms: finite freeness bounds the degree by $p$, while the automorphisms force degree at least $p$. The [determinant](../../../../../../determinant.md) norm therefore equals the product of its conjugates. Norms commute with this scalar extension, so

$$
\varphi(Nf)=\prod_{\xi^p=1}f(\xi X-1)
$$

as required. Finally, any other unit-valued map satisfying this identity has the same image under $\varphi$ for every $f$, and injectivity of $\varphi$ makes it identical to $N$. **The Coleman norm operator exists and is unique.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
