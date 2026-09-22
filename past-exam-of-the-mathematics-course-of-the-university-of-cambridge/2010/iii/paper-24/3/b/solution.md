<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The intended statement uses a nontrivial [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md). Under that convention choose $t$ with $0<|t|<1$. A compact neighborhood $C$ of zero contains an open ball of some radius $r>0$. For sufficiently large $N$, $t^N\mathcal O_K$ is contained in that ball. The [valuation ring](../../../../../../valuation-ring.md) is closed, so $t^N\mathcal O_K$ is a closed subset of $C$ and is compact. Scaling shows that $\mathcal O_K$ itself is compact.

Its [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m=\{x:|x|<1\}$ is open. The [residue field](../../../../../../residue-field.md) $k=\mathcal O_K/\mathfrak m$ is therefore discrete and compact, hence finite: the open cover by its singleton sets has a finite subcover. Since $\mathfrak m$ has finite index, its complement is a finite union of open cosets. Thus $\mathfrak m$ is also closed and compact.

The continuous [absolute value on a field](../../../../../../absolute-value-algebra.md) attains its maximum on $\mathfrak m$. Nontriviality supplies a nonzero element there, so this maximum is $\rho=|\pi|$ for some $\pi\ne0$, with $0<\rho<1$. If $x\in\mathfrak m$, then $|x/\pi|\leq1$, so $\mathfrak m=\pi\mathcal O_K$.

For arbitrary $x\ne0$, choose the integer $n$ for which $\rho^{n+1}<|x|\leq\rho^n$. Then $\rho<|x/\pi^n|\leq1$. This element cannot lie in $\mathfrak m$, by maximality of $\rho$, so its [absolute value on a field](../../../../../../absolute-value-algebra.md) is one. Therefore $|x|=\rho^n$. This proves [discrete valuation from nontrivial local compactness](../../../../../../discrete-valuation-from-nontrivial-local-compactness.md):

$$
\boxed{|K^\times|=\rho^{\mathbb Z},\qquad k\text{ finite}.}
$$

The [nontrivial valuation in the local compactness criterion](../../../../../../nontrivial-valuation-in-the-local-compactness-criterion.md) is essential. If the [trivial absolute value](../../../../../../trivial-absolute-value.md) is admitted, the displayed source claim is false: take $\mathbb Q$ with that [absolute value on a field](../../../../../../absolute-value-algebra.md). It is complete and discrete, hence locally compact, but its [valuation ring](../../../../../../valuation-ring.md) and [residue field](../../../../../../residue-field.md) are both $\mathbb Q$, which is infinite. The intended nontrivial case has been proved above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
