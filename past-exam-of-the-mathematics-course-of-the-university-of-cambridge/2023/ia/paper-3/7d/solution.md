<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The map $H\times K\to HK$, $(h,k)\mapsto hk$, has fibers of size $|H\cap K|$: two pairs have the same product exactly when their quotient is represented by an element of the intersection. Hence

$$
|HK|=\frac{|H||K|}{|H\cap K|}.
$$

The standard intersection-index inequality gives $[G:H\cap K]\leq [G:H][G:K]=ab$. This index is divisible by both coprime numbers $a$ and $b$, so it equals $ab$. The displayed formula then gives $|HK|=|G|$, hence $HK=G$.

The conjugacy class and centralizer are

$$
\operatorname{Conj}_G(x)=\{g^{-1}xg:g\in G\},
\qquad C_G(x)=\{g:gx=xg\},
$$

and orbit--stabilizer gives $|\operatorname{Conj}_G(x)|=[G:C_G(x)]$. Thus the coprimality hypothesis gives $C_G(x)C_G(y)=G$.

One inclusion in the desired equality follows by conjugating $xy$. Conversely take $g^{-1}xg\,h^{-1}yh$. Write $hg^{-1}=ab$ with $a\in C_G(y)$ and $b\in C_G(x)$. The hint then rewrites the product as

$$
h^{-1}a(xy)a^{-1}h,
$$

which is conjugate to $xy$. Therefore

$$
\boxed{\operatorname{Conj}_G(xy)=
\operatorname{Conj}_G(x)\operatorname{Conj}_G(y).}
$$

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
