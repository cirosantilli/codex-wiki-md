<h1 id="18f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put

$$
\delta=\sqrt c,
\qquad
\beta=\frac{\delta}{\alpha}.
$$

The four roots are $\alpha,-\alpha,\beta,-\beta$. If $\delta\in\mathbb Q(\alpha)$, then

$$
K=\mathbb Q(\alpha),
\qquad
[K:\mathbb Q]=4,
$$

because $g$ is irreducible. Hence the Galois group has order four and acts transitively, hence regularly, on the roots.

Let $\tau$ be the automorphism taking $\alpha$ to $\beta$. Since $\tau(\delta)=\pm\delta$,

$$
\tau^2(\alpha)
=\tau\left(\frac{\delta}{\alpha}\right)
=\frac{\tau(\delta)}{\beta}
=\begin{cases}
\alpha,&\tau(\delta)=\delta,\\
-\alpha,&\tau(\delta)=-\delta.
\end{cases}
$$

If $\tau(\delta)=\delta$, then $\tau$ is an involution. Together with the distinct involution taking $\alpha$ to $-\alpha$, it gives

$$
\boxed{\operatorname{Gal}(K/\mathbb Q)\cong C_2\times C_2.}
$$

In the ordered root set $(\alpha,-\alpha,\beta,-\beta)$ these generators act as double transpositions.

If $\tau(\delta)=-\delta$, then

$$
\alpha\longmapsto\beta\longmapsto-\alpha
\longmapsto-\beta\longmapsto\alpha,
$$

so $\tau$ has order four and

$$
\boxed{\operatorname{Gal}(K/\mathbb Q)\cong C_4.}
$$

This is the degree-four case in the [Galois group of an irreducible even quartic](../../../../../../galois-group-of-an-irreducible-even-quartic.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [18F](../../18f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
