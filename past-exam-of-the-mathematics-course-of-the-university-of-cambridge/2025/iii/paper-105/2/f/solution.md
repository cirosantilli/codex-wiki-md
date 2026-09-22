<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md) says that if $U\subset\mathbb R^n$ is a bounded Lipschitz domain, then

$$
W^{1,p}(U)\Subset L^q(U)
$$

for $1\leq q<p^*=np/(n-p)$ when $p<n$. When $p=n$, the embedding is compact into every finite $L^q$, and when $p>n$ it is compact into $C^0(\overline U)$, hence into every $L^q$.

The boundedness of the domain is essential. Choose a nonzero $\phi\in C_c^\infty(0,1)$ and set

$$
u_j(x)=\phi(x-2j)
\qquad(x>0).
$$

Translation invariance gives $\|u_j\|_{W^{1,1}(\mathbb R_+)}=\|\phi\|_{W^{1,1}}$, so after a fixed rescaling these functions lie in the unit ball. Their supports are pairwise disjoint and

$$
\|u_j-u_k\|_{L^1(\mathbb R_+)}=2\|\phi\|_{L^1}
\qquad(j\ne k).
$$

**No subsequence is [Cauchy](../../../../../../cauchy-sequence.md) in $L^1$, so the unit ball is not compact.** This is the standard [failure of Rellich compactness on an unbounded domain](../../../../../../failure-of-rellich-compactness-on-an-unbounded-domain.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
