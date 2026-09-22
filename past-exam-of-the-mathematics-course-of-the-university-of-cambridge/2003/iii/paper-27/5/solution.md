<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Here projection means [Hermitian](../../../../../hermitian-operator.md) [orthogonal projection](../../../../../orthogonal-projection.md): $P=P^*=P^2$ with $\operatorname{tr}P=k$, as indicated by the unitary conjugation in the question. These matrices represent the [complex Grassmannian as orthogonal projections](../../../../../complex-grassmannian-as-orthogonal-projections.md), a compact manifold of complex dimension $k(n-k)$. The constants $c_i$ are real. Let $A^*=-A$ and use the given tangent directions $[A,P]$. Cyclicity of the [matrix trace](../../../../../matrix-trace.md) gives

$$
df_P([A,P])=\operatorname{tr}(C[A,P])=\operatorname{tr}([P,C]A).
$$

The [commutator](../../../../../commutator.md) $B=[P,C]$ is skew-Hermitian. If this derivative vanishes for every skew-Hermitian $A$, choose $A=B$ to obtain

$$
0=\operatorname{tr}(B^2)=-\operatorname{tr}(B^*B),
$$

so $B=0$. Conversely $[P,C]=0$ makes every tangent derivative zero. Because the diagonal entries of $C$ are distinct, a commuting [matrix](../../../../../matrix.md) $P$ is diagonal. Its idempotent entries are zero or one. Thus the critical projections are exactly

$$
\boxed{P_I=\operatorname{diag}(\mathbf1_{1\in I},\ldots,\mathbf1_{n\in I}),\qquad |I|=k,}
$$

with $\binom nk$ [critical points](../../../../../critical-point.md) and values $f(P_I)=\sum_{i\in I}c_i$.

To compute the [Hessian matrix](../../../../../hessian-matrix.md), write $E=\operatorname{span}\{e_i:i\in I\}$ and $E^\perp=\operatorname{span}\{e_j:j\notin I\}$. A neighboring plane is the graph of a complex [linear map](../../../../../linear-map.md) $Z:E\to E^\perp$. With $W=\binom I Z$, its orthogonal projection is $P(Z)=W(I+Z^*Z)^{-1}W^*$. Writing $C_E,C_{E^\perp}$ for the diagonal blocks, we get

$$
f(P(Z))=\operatorname{tr}\bigl(C_E(I+Z^*Z)^{-1}\bigr)+\operatorname{tr}\bigl(C_{E^\perp}Z(I+Z^*Z)^{-1}Z^*\bigr).
$$

Expanding $(I+Z^*Z)^{-1}=I-Z^*Z+O(\|Z\|^4)$ yields

$$
f(P(Z))=f(P_I)+\sum_{i\in I,\ j\notin I}(c_j-c_i)|z_{ji}|^2+O(\|Z\|^4).
$$

Each complex coordinate has two real components, each with Hessian coefficient $2(c_j-c_i)$. Every coefficient is nonzero, proving that $f$ is a [Morse function](../../../../../morse-function.md). Its negative directions correspond to $j<i$. For $I=\{i_1<\cdots<i_k\}$ there are $i_a-a$ complementary indices below $i_a$, giving

$$
\boxed{\operatorname{ind}(P_I)=2\#\{(i,j):i\in I,\ j\notin I,\ j<i\}=2\sum_{a=1}^k(i_a-a).}
$$

This is the [diagonal trace Morse function on a complex Grassmannian](../../../../../diagonal-trace-morse-function-on-a-complex-grassmannian.md). Its critical values need not be distinct; ties between sums do not make its critical points degenerate.

All [Morse indices](../../../../../morse-index.md) are even. Choose a [Morse-Smale gradient flow](../../../../../morse-smale-gradient-flow.md) and form its integral [Morse chain complex](../../../../../morse-chain-complex.md). The odd-degree chain groups vanish, so every differential vanishes. Equivalently the [Morse handle-attachment theorem](../../../../../morse-handle-attachment-theorem.md) supplies only even-dimensional cells. The [integral homology of complex Grassmannians](../../../../../integral-homology-of-complex-grassmannians.md) is therefore

$$
\boxed{H_{2r}(\operatorname{Gr}(k,n);\mathbb Z)=\mathbb Z^{N_r},\quad H_{2r+1}(\operatorname{Gr}(k,n);\mathbb Z)=0,}
$$

where $N_r$ counts the subsets with $\sum_a(i_a-a)=r$, and $0\leq r\leq k(n-k)$. In particular there is no torsion. The nondecreasing sequence $i_a-a$ lies between zero and $n-k$, so reversing it identifies these subsets with [partitions of an integer](../../../../../partition-of-an-integer.md) $r$ fitting in a $k$ by $(n-k)$ rectangle. The [Poincaré polynomial](../../../../../poincare-polynomial.md) is explicitly

$$
\sum_{|I|=k}t^{2\sum_a(i_a-a)}.
$$

For the permitted example $\operatorname{Gr}(2,4)$, the subsets $12,13,14,23,24,34$ have indices $0,2,4,4,6,8$. Thus

$$
\boxed{H_0=H_2=H_6=H_8=\mathbb Z,\quad H_4=\mathbb Z^2,\quad H_{\mathrm{odd}}=0.}
$$

The general calculation above applies throughout $2\leq k\leq n-2$; it does not reduce to any of the excluded rank-one cases.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
