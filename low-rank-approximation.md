# Low-rank approximation

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Low-rank_approximation)

A low-rank approximation replaces an $m\times n$ [matrix](matrix.md) $A$ by a [matrix](matrix.md) $B$ of [matrix rank](matrix-rank.md) at most a chosen integer $r$, with $0\leq r\leq\min(m,n)$, while making an explicitly chosen error [norm](norm.md) small. The point is to describe many entries using a few shared patterns: an [image compression](image-compression.md) may retain broad brightness patterns while discarding finer ones. The approximation is useful when the saved storage or computation justifies the lost detail. A small [matrix rank](matrix-rank.md) alone says nothing about the error.

The compact representation is a sum of [outer products](outer-product.md), equivalently a product of two thin [matrices](matrix.md):

$$
B=XY^*=\sum_{j=1}^r x_jy_j^*,\qquad
X\in\mathbb C^{m\times r},\quad Y\in\mathbb C^{n\times r}.
$$

Here $x_j,y_j$ are the columns of $X,Y$, and the star denotes the [conjugate transpose](conjugate-transpose.md); over the [real numbers](real-number.md) use the [transpose](transpose.md). The [rank bound for a matrix product](rank-bound-for-a-matrix-product.md) gives $\operatorname{rank}B\leq r$. Conversely, choose a [basis](basis.md) of the [column space](column-space.md) of $B$ as the columns of $X$, and put the coordinates of each column of $B$ into $Y^*$; pad with zero columns if the [matrix rank](matrix-rank.md) is smaller than $r$. Each nonzero [outer product](outer-product.md) is a [rank-one matrix](rank-one-matrix.md): it repeats a single column pattern at different strengths across the columns.

Keeping the two factors stores $r(m+n)$ [scalars](scalar.md) instead of $mn$. This saves space only when $r(m+n)<mn$. The usual [singular value decomposition](singular-value-decomposition.md) representation stores $r(m+n+1)$ [scalars](scalar.md) because it keeps the $r$ [singular values](singular-value.md) separately; absorbing them into one factor removes that extra array. These are representation sizes at equal [scalar](scalar.md) precision, before file overhead. See [Uschmajew and Vandereycken, §9.2: thin factors and their storage](https://link.springer.com/chapter/10.1007/978-3-030-31351-7_9), and [Illinois CS 357, Low-rank approximation: storing singular vectors and values](https://cs357.cs.illinois.edu/notes/ref-16-svd.html).

The factors also give $Bz=X(Y^*z)$ without forming the full [matrix](matrix.md) $B$. Direct evaluation uses $nr+mr$ [scalar](scalar.md) multiplications, compared with $mn$ for a dense [matrix](matrix.md) applied to a [vector](vector.md). For $m=1000,n=800,r=10$, the two factors contain $18{,}000$ [scalars](scalar.md) rather than $800{,}000$, and the same counts describe these multiplication costs. Constructing the factors is a separate cost. Moreover, a [low-rank approximation](low-rank-approximation.md) need not be a [sparse matrix](sparse-matrix.md): the constant $8\times8$ [matrix](matrix.md) whose entries are all $1$ has [matrix rank](matrix-rank.md) $1$ despite having no zero entries.

For the standard unweighted problem, write a [singular value decomposition](singular-value-decomposition.md) with $p=\min(m,n)$ and [singular values](singular-value.md) $\sigma_1\geq\cdots\geq\sigma_p\geq0$. Retain the first $r$ paired [left singular vectors](left-singular-vector.md) and [right singular vectors](right-singular-vector.md):

$$
A_r=\sum_{j=1}^r\sigma_j u_jv_j^*,\qquad A_0=0.
$$

The [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md) says that this same $A_r$ minimizes both of the following error [norms](norm.md) over all [matrices](matrix.md) with [matrix rank](matrix-rank.md) at most $r$:

$$
\min_{\operatorname{rank}B\leq r}\|A-B\|_F
=\|A-A_r\|_F=\left(\sum_{j=r+1}^p\sigma_j^2\right)^{1/2},
\qquad
\min_{\operatorname{rank}B\leq r}\|A-B\|_2
=\|A-A_r\|_2=\sigma_{r+1},
$$

where $\sigma_{p+1}=0$ and an empty sum is zero. Here the [Frobenius norm](frobenius-norm.md) is $\|E\|_F=(\sum_{i,j}|E_{ij}|^2)^{1/2}$, whereas the [operator norm](operator-norm.md) is specifically induced by the [Euclidean norm](euclidean-norm.md), $\|E\|_2=\max_{\|z\|_2=1}\|Ez\|_2$. The first aggregates errors in all entries; the second bounds the worst output error for a [unit vector](unit-vector.md) input. These formulas apply to real and complex [matrices](matrix.md). [Mazeika, §§4.1 and 4.3: norms and optimal singular-value truncation](https://math.uchicago.edu/~may/REU2016/REUPapers/Mazeika.pdf)

For $A\ne0$, a relative [Frobenius norm](frobenius-norm.md) tolerance $\varepsilon$ is met precisely when the discarded squared [singular values](singular-value.md) sum to at most $\varepsilon^2\sum_j\sigma_j^2$. Thus one can choose the smallest suitable $r$ before reconstructing the [matrix](matrix.md). Many individually small discarded [singular values](singular-value.md) can still have a large combined error. An [operator norm](operator-norm.md) tolerance instead tests only the largest discarded [singular value](singular-value.md), $\sigma_{r+1}$. The two questions can therefore select different ranks.

The following stipulated $8\times8$ [matrix](matrix.md) makes the tradeoff visible. Define four real [vectors](vector.md) of length $8$:

$$
h_0=(1,1,1,1,1,1,1,1)^T,\quad
h_1=(1,1,1,1,-1,-1,-1,-1)^T,
$$



$$
h_2=(1,1,-1,-1,1,1,-1,-1)^T,\quad
h_3=(1,-1,1,-1,1,-1,1,-1)^T,
\qquad
A=h_0h_0^T+\frac38h_1h_1^T+\frac18h_2h_2^T+\frac1{16}h_3h_3^T.
$$

The [vectors](vector.md) $h_j/\sqrt8$ are [orthonormal](orthonormal-set.md), so this is already a [singular value decomposition](singular-value-decomposition.md) written as [outer products](outer-product.md), with positive [singular values](singular-value.md) $8,3,1,1/2$. All entries lie between $7/16$ and $25/16$ and can be displayed as brightnesses. The first component is uniform brightness, the second distinguishes broad blocks, and the last two supply finer alternating patterns. This is a designed arithmetic example, not measured image data.

<a id="image-shared-patterns-in-a-stipulated-8-times8-matrix"></a>
![](low-rank-pattern-reconstruction.png)

**[Figure 13](#image-shared-patterns-in-a-stipulated-8-times8-matrix). Shared patterns in a stipulated $8\times8$ matrix**. The first three panels use the same brightness scale. Rank one retains uniform brightness; rank two adds the broad blocks. The signed residual $A-A_2$ has its own color scale to expose the discarded patterns. The factors apply a [linear map](linear-map.md) through just $r$ intermediate coordinates.

Here $A_1=h_0h_0^T$ has every entry equal to $1$, while $A_2=h_0h_0^T+3h_1h_1^T/8$ has entries $11/8$ within the two diagonal blocks and $5/8$ in the other two blocks. For instance, $A_{11}=25/16$ becomes $(A_2)_{11}=11/8$: its error is $3/16$. The full residual is $h_2h_2^T/8+h_3h_3^T/16$, whose [Frobenius norm](frobenius-norm.md) is $\sqrt{1+(1/2)^2}=\sqrt5/2$ and whose [operator norm](operator-norm.md) is $1$. Since $\|A\|_F=\sqrt{297}/2$, the relative [Frobenius norm](frobenius-norm.md) error is $\sqrt{5/297}\approx12.97\%$. Two thin factors use $32$ [scalars](scalar.md), or $34$ if the normalized [left singular vectors](left-singular-vector.md), [right singular vectors](right-singular-vector.md), and [singular values](singular-value.md) are stored separately, instead of $64$ dense entries.

<a id="image-error-falls-as-storage-rises-for-the-stipulated-matrix"></a>
![](low-rank-error-storage-tradeoff.png)

**[Figure 14](#image-error-falls-as-storage-rises-for-the-stipulated-matrix). Error falls as storage rises for the stipulated matrix**. The exact [Frobenius norm](frobenius-norm.md) and [operator norm](operator-norm.md) errors are plotted for $r=0,1,2,3,4$. The storage panel counts the two thin factors, or the normalized [left singular vectors](left-singular-vector.md) and [right singular vectors](right-singular-vector.md) plus separate [singular values](singular-value.md), at equal [scalar](scalar.md) precision. Lines join discrete rank choices; they do not represent intermediate ranks or measured data.

Retaining three components reduces the [Frobenius norm](frobenius-norm.md) error to $1/2$ while using $48$ [scalars](scalar.md) in two factors. Retaining all four reconstructs $A$ exactly but uses $64$ [scalars](scalar.md), giving no saving in this generic representation; keeping the [singular values](singular-value.md) separately uses $68$. Our particular sign patterns could be encoded more economically, but that would exploit an additional structure beyond the general [low-rank approximation](low-rank-approximation.md). The striking feature is that numerical error and storage can both be read from the decomposition, rather than judged only by how smooth the picture looks.

The constraint is deliberately [matrix rank](matrix-rank.md) _at most_ $r$. The truncation has $\operatorname{rank}A_r=\min(r,\operatorname{rank}A)$. If $\operatorname{rank}A<r$, the best approximation is $A$ itself, with zero error. Requiring [matrix rank](matrix-rank.md) exactly $r$ can destroy attainment: for $A=\operatorname{diag}(1,0)$ and $r=2$, the [matrices](matrix.md) $B_\delta=\operatorname{diag}(1,\delta)$ have [matrix rank](matrix-rank.md) $2$ for $\delta>0$, and both error [norms](norm.md) equal $\delta$. Their error has [infimum](infimum.md) zero, but no rank-two [matrix](matrix.md) attains it. If $r\leq\operatorname{rank}A$, the displayed $A_r$ does have [matrix rank](matrix-rank.md) exactly $r$ and attains the same minimum under either constraint.

Optimality also does not always mean uniqueness. For $0<r<\operatorname{rank}A$, the best [Frobenius norm](frobenius-norm.md) approximation is unique when $\sigma_r>\sigma_{r+1}$. [Uschmajew and Vandereycken, Theorem 9.1: uniqueness across a singular-value gap](https://link.springer.com/chapter/10.1007/978-3-030-31351-7_9) A positive tie across the cutoff permits different choices: for $A=\operatorname{diag}(3,3,1)$ and $r=1$, both $\operatorname{diag}(3,0,0)$ and $\operatorname{diag}(0,3,0)$ have [Frobenius norm](frobenius-norm.md) error $\sqrt{10}$ and [operator norm](operator-norm.md) error $3$. More generally, $3ww^T$ is optimal for every real [unit vector](unit-vector.md) $w$ in the first two coordinate directions. Rotating which tied direction is kept changes the approximation. Repeated [singular values](singular-value.md) entirely inside the retained group do not change its sum of [outer products](outer-product.md). At $r=0$ the only feasible [matrix](matrix.md) is zero; at $r\geq\operatorname{rank}A$ the unique zero-error approximation is $A$, even if some [singular values](singular-value.md) are tied at zero.

A strict gap does not guarantee uniqueness for the [operator norm](operator-norm.md). For $A=\operatorname{diag}(3,1)$ and $r=1$, every $B_t=\operatorname{diag}(t,0)$ with $2\leq t\leq4$ has [matrix rank](matrix-rank.md) $1$ and error $\|A-B_t\|_2=\max(|3-t|,1)=1$, which is optimal. Only $t=3$ minimizes the [Frobenius norm](frobenius-norm.md), since $\|A-B_t\|_F=\sqrt{(3-t)^2+1}$. An unchanged worst direction can hide extra error in another direction under the [operator norm](operator-norm.md).

Finally, these guarantees concern the stated [norms](norm.md) and the sole [matrix rank](matrix-rank.md) constraint. They do not establish that a discarded pattern is noise or irrelevant to a particular task: the finer patterns in our constructed example were put there intentionally. Adding entrywise weights or restrictions on the factors changes the problem, so the [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md) above does not automatically solve it. For historical context, the original 1936 matrix problem is documented in the existing [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md) section.

**Table of contents**

- [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Low-rank approximation](low-rank-approximation.md)
- [Singular value decomposition](singular-value-decomposition.md)
