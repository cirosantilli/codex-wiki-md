<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
C_n=\overline{W(Q_nAQ_n^*)}.
$$

The tail spaces decrease, so $C_{n+1}\subseteq C_n$. If $\lambda\in\bigcap_nC_n$, choose a unit vector $v_n$ supported after coordinate $n$ with $|\langle Av_n,v_n\rangle-\lambda|<1/n$. Such vectors converge weakly to zero, hence $\lambda\in W_e(A)$.

Conversely, if $v_j\rightharpoonup0$ and $\langle Av_j,v_j\rangle\to\lambda$, then for every fixed $n$ the first $n$ coordinates of $v_j$ tend to zero. After normalizing $Q_nv_j$, its numerical values still tend to $\lambda$, so $\lambda\in C_n$. Therefore

$$
\boxed{\bigcap_{n=1}^\infty C_n=W_e(A)}.
$$

When the intersection is nonempty, decreasing closed sets have distance functions increasing pointwise to the distance from their intersection; on each compact set this convergence is uniform. This is precisely

$$
\boxed{C_n\downarrow W_e(A)
\quad\text{in the <Attouch--Wets topology>}}.
$$

If $W_e(A)=\varnothing$ and a compact $K$ met every $C_n$, nestedness and compactness would supply a convergent sequence whose limit belongs to all $C_n$, a contradiction. Hence $K\cap C_n=\varnothing$ for all sufficiently large $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
