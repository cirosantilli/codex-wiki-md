<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The proposed implication is not symmetric. In $X=\mathbb R$, take

$$
A=\{0,2\},\qquad B=\{0\},\qquad r=1.
$$

Then $B\subseteq E_1(A)$, but $2\notin E_1(B)$, so $A\nsubseteq E_1(B)$.

For a point and a nonempty set, write $d(x,B)=\inf_{b\in B}d(x,b)$. The given [Hausdorff distance](../../../../../../hausdorff-distance.md) is equivalently

$$
d_H(A,B)=\max\left\{
\sup_{a\in A}d(a,B),
\sup_{b\in B}d(b,A)
\right\}.
$$

It is nonnegative and symmetric. If $d_H(A,B)=0$, then every $a\in A$ has $d(a,B)=0$, so $a\in\overline B=B$ because $B$ is closed; hence $A\subseteq B$, and symmetry gives $A=B$.

For the triangle inequality, the ordinary triangle inequality gives

$$
d(a,C)\leq d(a,B)+\sup_{b\in B}d(b,C).
$$

Taking suprema over $a\in A$, and then repeating with $A$ and $C$ interchanged, yields

$$
d_H(A,C)\leq d_H(A,B)+d_H(B,C).
$$

Thus $d_H$ is a metric on $H(X)$. Closedness is essential: if it is omitted, then the distinct bounded sets $(0,1)$ and $[0,1]$ have Hausdorff distance zero.

For singleton sets,

$$
d_H(\{x\},\{y\})=d(x,y),
$$

so $\theta(x)=\{x\}$ is an isometry. Its image is closed. Indeed, if $\{x_n\}$ converges in Hausdorff distance to $A\in H(X)$, then for every $\varepsilon>0$ and all sufficiently large $n$,

$$
A\subseteq E_\varepsilon(\{x_n\}).
$$

Hence any $a,b\in A$ satisfy $d(a,b)\leq d(a,x_n)+d(x_n,b)\leq2\varepsilon$. Letting $\varepsilon\downarrow0$ gives $a=b$, so the nonempty set $A$ is a singleton. This is the [closed singleton embedding in a Hausdorff hyperspace](../../../../../../closed-singleton-embedding-in-a-hausdorff-hyperspace.md).

If $H(X)$ is complete, its closed subspace $\theta(X)$ is complete. Since $\theta$ is an isometry, $X$ is complete. Hence [completeness is reflected by the Hausdorff hyperspace](../../../../../../completeness-is-reflected-by-the-hausdorff-hyperspace.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
