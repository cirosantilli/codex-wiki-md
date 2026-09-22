<h1 id="20f/solution">Solution</h1>

↑ **Parent:** [20F](../20f.md)

Put $s=\sqrt{-17}$. The [ring of integers of a number field](../../../../../ring-of-integers.md) is $\mathbb Z[s]$ and the [field discriminant](../../../../../field-discriminant.md) is $-68$. The [Minkowski bound for ideal classes](../../../../../minkowski-s-bound.md) says that each [ideal class](../../../../../ideal-class.md) has an integral ideal representative of norm at most $(2/\pi)\sqrt{68}<6$.

The prime two ramifies as $(2)=\mathfrak p_2^2$, where $\mathfrak p_2=(2,1+s)$. Three splits as $(3)=\mathfrak p_3\overline{\mathfrak p}_3$, choosing $\mathfrak p_3=(3,1+s)$, whereas five is inert because $-17\equiv3\pmod5$ is not a square. The norm bound therefore leaves only the classes of $1$, $\mathfrak p_2$, $\mathfrak p_3$ and $\overline{\mathfrak p}_3$; a norm-four ideal is $\mathfrak p_2^2$ and is principal.

The ideal $\mathfrak p_2$ is not principal, since an element of norm two would solve $a^2+17b^2=2$. On the other hand $N(1+s)=18$, and $1+s$ is divisible by $\mathfrak p_2$ and $\mathfrak p_3$ but not $\overline{\mathfrak p}_3$. Unique [prime ideal factorization](../../../../../prime-ideal-factorization.md) and the norm give $(1+s)=\mathfrak p_2\mathfrak p_3^2$. Thus $[\mathfrak p_3]^2=[\mathfrak p_2]$, which has order two, and

$$
\boxed{\operatorname{Cl}(\mathbb Q(\sqrt{-17}))\cong C_4.}
$$

For the Diophantine equation, $x$ must be positive. If $x$ were even, $y^2\equiv15\pmod{32}$, impossible for a square. Thus $x$ is odd and $y$ even. If $17\mid x$, then $17\mid y$, but $y^2+17$ would have 17-adic valuation one while $x^5$ has valuation divisible by five, also impossible.

The ideals $(y+s)$ and $(y-s)$ are consequently coprime. A common prime divides $2s$ and hence lies over two or seventeen, both excluded above. Their product is $(x)^5$, so unique [prime ideal factorization](../../../../../prime-ideal-factorization.md) gives $(y+s)=\mathfrak a^5$. Since the [ideal class group](../../../../../ideal-class-group.md) has order four, $[\mathfrak a]^5=1$ forces $[\mathfrak a]=1$. Write $\mathfrak a=(a+bs)$ with integers $a,b$. The only units are $\pm1$ by their norm, and the sign can be absorbed into the fifth power. Hence $y+s=(a+bs)^5$.

Comparing the coefficient of $s$ gives

$$
1=b(5a^4-170a^2b^2+289b^4),\qquad b=\pm1.
$$

For $b=1$, the bracket would be one, but it is four modulo five. For $b=-1$, the bracket would be minus one, but it is one modulo three for either possible square residue of $a$. Both cases are impossible. Therefore **there are no integer solutions**.

## ↑ Ancestors (11)

1. [20F](../20f.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
