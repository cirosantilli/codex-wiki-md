<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The algebraic [dual map](../../../../../../transpose-of-a-linear-map.md) is $\delta=\alpha^\vee:W^*\to V^*$, defined by $\delta(\varphi)=\varphi\circ\alpha$. The [annihilator of a vector subspace](../../../../../../annihilator-of-a-vector-subspace.md) $U\subseteq V$ is

$$
U^\circ=\{\lambda\in V^*: \lambda(u)=0\text{ for all }u\in U\}.
$$

Every functional $\varphi\circ\alpha$ vanishes on $\ker\alpha$, so $\operatorname{im}\delta\subseteq(\ker\alpha)^\circ$. Conversely, let $\lambda\in(\ker\alpha)^\circ$. Define a functional on $\operatorname{im}\alpha$ by $\widetilde\lambda(\alpha v)=\lambda(v)$. It is well defined because two preimages differ by an element of $\ker\alpha$. Extend a [basis](../../../../../../basis.md) of $\operatorname{im}\alpha$ to one of $W$ and extend the functional arbitrarily, for instance by zero on the extra basis vectors. The resulting $\varphi\in W^*$ satisfies $\delta\varphi=\lambda$.

This is the [dual image and kernel annihilator identity](../../../../../../dual-image-and-kernel-annihilator-identity.md). Therefore

$$
\boxed{\operatorname{im}\delta=(\ker\alpha)^\circ.}
$$

The [basis extension](../../../../../../basis-extension.md) theorem also gives $\dim U^\circ=\dim V-\dim U$. By the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md),

$$
\boxed{\dim\operatorname{im}\delta=\dim V-\dim\ker\alpha=\dim\operatorname{im}\alpha.}
$$

Apply [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) to both maps, using $\dim W^*=\dim W$, to obtain

$$
\boxed{\dim\ker\alpha-\dim\ker\delta=\dim V-\dim W.}
$$

Over $\mathbb C$, this is the algebraic dual, without complex conjugation; the [adjoint operator](../../../../../../adjoint-operator.md) in part (b) uses the inner products instead.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
