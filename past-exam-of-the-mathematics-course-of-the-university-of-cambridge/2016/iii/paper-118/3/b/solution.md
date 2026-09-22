<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the convention that the [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) is conjugate-linear in its first argument. In a [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md) $e=(e_1,\ldots,e_r)$, let $H_{ij}=h(e_i,e_j)$, so $h(ev,ew)=v^\dagger Hw$. Write $De=e\theta$, or equivalently $D(ev)=e(dv+\theta v)$.

Compatibility with the [holomorphic vector bundle](../../../../../../holomorphic-vector-bundle.md) structure means $D^{0,1}=\bar\partial_E$. Since the frame is holomorphic, this forces $\theta^{0,1}=0$. [Metric compatibility](../../../../../../metric-compatibility.md) means

$$
dh(s,t)=h(Ds,t)+h(s,Dt),
$$

or, in the chosen frame, $dH=\theta^\dagger H+H\theta$. Conjugate transpose here also conjugates the one-form factors. Taking the $(1,0)$ component gives $\partial H=H\theta$, and hence

$$
\boxed{\theta=H^{-1}\partial H.}
$$

This proves uniqueness and suggests existence. The proposed $\theta$ has type $(1,0)$, and its conjugate transpose obeys $\theta^\dagger H=\bar\partial H$, since $H=H^\dagger$. Therefore $dH=\theta^\dagger H+H\theta$, proving [metric compatibility](../../../../../../metric-compatibility.md) as well.

Under a change of [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md) $e'=eG$, we have $H'=G^\dagger HG$ and $\partial G^\dagger=0$. A direct computation yields

$$
(H')^{-1}\partial H'=G^{-1}\theta G+G^{-1}\partial G.
$$

Because $G$ is holomorphic, $\partial G=dG$; this is exactly the transformation rule for a [connection one-form](../../../../../../connection-one-form.md). The locally defined connections therefore glue to a global [connection on a vector bundle](../../../../../../connection-vector-bundle.md). **The Chern connection exists uniquely**, and its [local formula for the Chern connection on a vector bundle](../../../../../../local-formula-for-the-chern-connection-on-a-vector-bundle.md) is

$$
\boxed{D=d+H^{-1}\partial H,\qquad D^{0,1}=\bar\partial_E.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
