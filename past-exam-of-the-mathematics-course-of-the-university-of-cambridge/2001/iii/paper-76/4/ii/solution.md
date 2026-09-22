<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $k\ge2$, the following precise [cardinality-controlled cyclic Freiman model](../../../../../../cardinality-controlled-cyclic-freiman-model.md) suffices. If $A\subseteq\mathbb Z$ is nonempty, $|A|=n$ and $D=kA-kA$ has $|D|\le Cn$, there is $A'\subseteq A$ with

$$
\boxed{|A'|\ge\frac n{k+1},\qquad A'\cong_k B\subseteq\mathbb Z_N,\qquad N=4|D|+1\le4Cn+1.}
$$

Here $\cong_k$ means a bijection preserving and reflecting all equalities of $k$-term sums, a [Freiman s-isomorphism](../../../../../../freiman-s-isomorphism.md) of order $s=k$. The same construction works for $k=1$ if only injectivity is needed.

Choose an auxiliary prime $P$ larger than $N$ and every nonzero absolute value in $D$, and large enough to embed the finite set $A$ injectively modulo $P$. Multiply its residues by a uniformly chosen nonzero residue $u$. For a fixed $d\in D\setminus\{0\}$, $ud$ is uniform among the $P-1$ nonzero residues. The forbidden residues are

$$
\mathcal F=\{tN\pmod P:0<|tN|<P\},
$$

of number at most $2(P-1)/N$. The [union bound](../../../../../../boole-s-inequality.md) says that the probability some nonzero $d\in D$ enters $\mathcal F$ is at most $2(|D|-1)/N<1$. Fix a multiplier avoiding every forbidden event.

Let $\widetilde a\in\{0,\ldots,P-1\}$ represent $ua\pmod P$. Partition that range into $k+1$ half-open intervals of length $P/(k+1)$ and retain the most populated interval; it supplies $A'$ with $|A'|\ge n/(k+1)$. Define the model map by $\theta(a)=\widetilde a\pmod N$. For two $k$-term sums of retained representatives, their difference $T$ has $|T|<P$. If the original sums are equal, then $T\equiv0\pmod P$, hence $T=0$, so the model preserves the equality.

Conversely, if the model sums are equal, then $T$ is a multiple of $N$. If their original difference $d\in D$ were nonzero, it would satisfy $ud\equiv T\pmod P$ with $0<|T|<P$, contradicting the forbidden-event choice. If $T=0$ directly, $ud\equiv0$ implies $d=0$ too by the choice of $P$. Thus the equality is reflected. Padding equal one-term images with $k-1$ copies of a fixed retained element shows that the map is injective. This proves the [Freiman s-isomorphism](../../../../../../freiman-s-isomorphism.md) and the claimed bound on the cyclic modulus, independently of the diameter of $A$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
