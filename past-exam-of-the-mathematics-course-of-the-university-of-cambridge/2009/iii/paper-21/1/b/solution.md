<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $I=(f_1,\ldots,f_r)$ and $\mathfrak m=(y_0,\ldots,y_n)$. If $\mathfrak m^N\subseteq I$, a projective common zero would have some coordinate $y_j\ne0$. For $N>0$, the polynomial $y_j^N\in I$ could not vanish there; for $N=0$, the inclusion puts $1$ in $I$, also impossible. Thus the projective zero set is empty.

Conversely, over an [algebraically closed field](../../../../../../algebraically-closed-field.md), emptiness of the projective zero set means the affine common zero set is contained in the origin. Every $y_j$ vanishes there, so the [Hilbert Nullstellensatz](../../../../../../hilbert-nullstellensatz.md) puts $y_j$ in $\sqrt I$. Choose integers $e_j\ge1$ with $y_j^{e_j}\in I$, and set

$$
N=1+\sum_{j=0}^n(e_j-1).
$$

Every degree-$N$ [monomial](../../../../../../monomial.md) has some exponent at least the corresponding $e_j$, by the pigeonhole principle, and is consequently in $I$. Those [monomials](../../../../../../monomial.md) generate $\mathfrak m^N$, proving

$$
\boxed{V_+(I)=\varnothing\iff\mathfrak m^N\subseteq I\text{ for some }N\ge0.}
$$

The argument includes the unit-ideal case. This proves the [Projective Nullstellensatz](../../../../../../projective-nullstellensatz.md) criterion directly from its affine counterpart.

Over a general field, this same criterion concerns geometric zeros: apply the proof after extension to an algebraic closure. Inclusion of each degree-$N$ [monomial](../../../../../../monomial.md) descends back to $k$, since its class in $k[y]/I$ is zero if and only if it becomes zero after a field extension; tensoring a [vector space](../../../../../../vector-space-split.md) with an extension field is faithful. If instead one counts only $k$-rational projective points, the assertion is false. For example $y_0^2+y_1^2$ has no real projective zero but has the complex zero $[1:i]$, so its [ideal](../../../../../../ideal.md) cannot contain any power of $\mathfrak m$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
