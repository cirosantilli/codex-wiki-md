<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $K=\mathbb Q(\sqrt{pq})$ and $E=\mathbb Q(\sqrt p,\sqrt q)$. The distinct primes give independent square classes, so $[E:\mathbb Q]=4$ and $[E:K]=2$. In particular $K(\sqrt p)=K(\sqrt q)=E$: these are the same quadratic extension of $K$. We prove it is [unramified](../../../../../../unramified-extension.md) by an explicit [field discriminant](../../../../../../field-discriminant.md) calculation.

Since $p,q\equiv1\pmod4$, put $a=(1+\sqrt p)/2$, $b=(1+\sqrt q)/2$. Both are [algebraic integers](../../../../../../algebraic-integer.md). The ring $R=\mathbb Z[a,b]\subseteq\mathcal O_E$ has basis $1,a,b,ab$. Up to the ordering of the basis, its [trace pairing](../../../../../../trace-pairing.md) matrix is the tensor product of the quadratic trace matrices, because the four embeddings of $E$ choose the two radical signs independently. The two quadratic matrices are

$$
T_p=\begin{pmatrix}2&1\\1&(p+1)/2\end{pmatrix},\qquad
T_q=\begin{pmatrix}2&1\\1&(q+1)/2\end{pmatrix},
\qquad \det T_p=p,\quad\det T_q=q.
$$

Thus

$$
\operatorname{disc}(R)=\det(T_p\otimes T_q)=p^2q^2.
$$

On the other hand, $pq$ is squarefree and congruent to one modulo four, so $d_K=pq$. Let $j=[\mathcal O_E:R]$. The [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md) and the [relative discriminant](../../../../../../relative-discriminant.md) tower formula give

$$
\frac{p^2q^2}{j^2}=d_E
=d_K^{[E:K]}N_{K/\mathbb Q}(\mathfrak d_{E/K})
=p^2q^2N_{K/\mathbb Q}(\mathfrak d_{E/K}).
$$

The [ideal norm](../../../../../../ideal-norm.md) on the right is a positive integer, while $j$ is a positive integer. Hence $N(\mathfrak d_{E/K})=1/j^2$ forces $j=1$ and $\mathfrak d_{E/K}=\mathcal O_K$. Its prime divisors are exactly the ramified finite primes, so **$E/K$ is unramified at every finite prime**, including primes above $2,p,q$. This also proves $d_E=p^2q^2$, agreeing with the [discriminant of a biquadratic field](../../../../../../discriminant-of-a-biquadratic-field.md) formula.

Every embedding of $E$ is real, so the real places of $K$ split as well. The extension is quadratic, hence abelian. The ordinary [Hilbert class field characterization](../../../../../../hilbert-class-field-characterization.md) therefore implies

$$
\boxed{\mathbb Q(\sqrt p,\sqrt q)\subseteq H_K.}
$$

Finally, the [Artin reciprocity map](../../../../../../artin-reciprocity-law.md) identifies $\operatorname{Cl}(K)$ with $\operatorname{Gal}(H_K/K)$. Restriction onto $\operatorname{Gal}(E/K)\simeq C_2$ is surjective, so the [ideal class group](../../../../../../ideal-class-group.md) has a quotient of order two. Therefore **$\boxed{|\operatorname{Cl}(K)|\text{ is even}}$.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
