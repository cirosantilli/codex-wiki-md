<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) says the following. Let $v$ be a [discrete valuation](../../../../../../discrete-valuation.md) on a complete field $K$. If $f\in\mathcal O_K[X]$ and

$$
v(f(x_0))>2v(f'(x_0)),
$$

then $f$ has a root $x\in\mathcal O_K$ satisfying $v(x-x_0)>v(f'(x_0))$.

To prove it, apply [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md):

$$
x_{n+1}=x_n-\frac{f(x_n)}{f'(x_n)}.
$$

The initial inequality says that the first correction has valuation greater than $v(f'(x_0))$. Taylor expansion then shows inductively that $v(f'(x_n))=v(f'(x_0))$, while the valuations of the corrections tend to infinity. Hence $(x_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). Completeness gives a limit $x$, and continuity gives $f(x)=0$.

Now decompose the multiplicative group as

$$
\mathbb Q_3^\times
=3^{\mathbb Z}\times\{\pm1\}\times U_1,
\qquad U_1=1+3\mathbb Z_3.
$$

The [P-adic valuation](../../../../../../p-adic-valuation.md) gives

$$
3^{\mathbb Z}/3^{3\mathbb Z}\cong\mathbb Z/3\mathbb Z,
$$

and cubing is the identity on $\{\pm1\}$. Put $U_2=1+9\mathbb Z_3$. Expansion gives $U_1^3\subseteq U_2$. Conversely, for $u=1+9a\in U_2$, choose $b\equiv a\pmod3$ and put $x_0=1+3b$. For $f(X)=X^3-u$,

$$
v_3(f(x_0))\geq3>2=2v_3(f'(x_0)),
$$

so the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) produces a cube root in $U_1$. Thus $U_1^3=U_2$. Finally,

$$
U_1/U_2\longrightarrow\mathbb Z/3\mathbb Z,
\qquad 1+3b\longmapsto b\pmod3,
$$

is an isomorphism. Combining the valuation and principal-unit factors proves the [cube-class group of the 3-adic numbers](../../../../../../cube-class-group-of-the-3-adic-numbers.md) identity

$$
\boxed{\mathbb Q_3^\times/(\mathbb Q_3^\times)^3
\cong\mathbb Z/3\mathbb Z\times\mathbb Z/3\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
