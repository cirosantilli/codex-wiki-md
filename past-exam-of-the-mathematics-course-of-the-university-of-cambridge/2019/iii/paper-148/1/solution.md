<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An element $t\in T$ is an [integral element](../../../../../integral-element.md) over $R$ when it satisfies a monic equation

$$
t^n+r_{n-1}t^{n-1}+\cdots+r_0=0,
\qquad r_i\in R.
$$

The extension $R\subseteq T$ is an [integral extension](../../../../../integral-extension.md) when every $t\in T$ is integral over $R$.

Let $P\in\operatorname{Spec}R$ and localize both rings at $S=R\setminus P$. The extension $R_P\subseteq S^{-1}T$ remains integral. Choose a maximal ideal $\mathfrak n$ of $S^{-1}T$. The [contraction of a maximal ideal under an integral extension](../../../../../contraction-of-a-maximal-ideal-under-an-integral-extension.md) is maximal, and the local ring $R_P$ has unique maximal ideal $PR_P$, so $\mathfrak n\cap R_P=PR_P$. Contracting $\mathfrak n$ back to $T$ produces $Q\in\operatorname{Spec}T$ with $Q\cap R=P$. This proves the [Lying-over theorem](../../../../../lying-over-theorem.md) and hence the surjectivity of

$$
\pi:\operatorname{Spec}T\longrightarrow\operatorname{Spec}R.
$$

Suppose $Q_1\subseteq Q_2$ and both contract to $P$. Quotient by $Q_1$ and localize the resulting integral domain at the nonzero elements of $R/P$. The localized ring is an integral domain integral over the field $\operatorname{Frac}(R/P)$, and is therefore itself a field. The localization of $Q_2/Q_1$ must consequently be zero; since the localized ring is a domain, $Q_2/Q_1=0$. Thus the [incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md) gives

$$
\boxed{Q_1=Q_2.}
$$

The [Krull dimension](../../../../../krull-dimension.md) of a ring is the supremum of the lengths of its strict chains of prime ideals. Incomparability makes the contraction of every strict prime chain in $T$ strict, so $\dim T\leq\dim R$. Conversely, start over the bottom prime of any chain in $R$ using lying over and lift each subsequent inclusion using the [going-up theorem](../../../../../going-up-theorem.md). Hence

$$
\boxed{\dim T=\dim R.}
$$

For the concrete surface, write $x,y,z$ for the residue classes of $X,Y,Z$ and put

$$
u=x-z,\qquad v=y-z.
$$

Then

$$
xy+yz+zx=uv+2(u+v)z+3z^2,
$$

and characteristic zero allows division by three. Therefore

$$
T\cong k[u,v][z]\big/\left(z^2+\frac23(u+v)z+\frac13uv\right).
$$

Division by the monic quadratic shows that $T$ is free over $k[u,v]$ with basis $1,z$. In particular, $u,v$ are algebraically independent and the requested [Noether normalization of the quadratic surface xy plus yz plus zx](../../../../../noether-normalization-of-the-quadratic-surface-xy-plus-yz-plus-zx.md) is

$$
\boxed{R=k[x-z,y-z]\cong k[U,V].}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 148](../../paper-148-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
