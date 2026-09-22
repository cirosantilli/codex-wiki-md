<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $h\in H$, define $\pi(h)(n)=hnh^{-1}$. Since $N$ is a [normal subgroup](../../../../../../../normal-subgroup.md), this sends $N$ into itself. It preserves multiplication, and its inverse is conjugation by $h^{-1}$, so it is an [group automorphism](../../../../../../../group-automorphism.md) of $N$. Moreover

$$
\pi(h_1h_2)(n)=h_1h_2n h_2^{-1}h_1^{-1}
=\bigl(\pi(h_1)\circ\pi(h_2)\bigr)(n).
$$

Thus $\pi:H\to\operatorname{Aut}(N)$ is a [group homomorphism](../../../../../../../group-homomorphism.md), induced by the [group action](../../../../../../../group-action-split.md) of [conjugation](../../../../../../../conjugation.md).

If $\pi$ is trivial, every element of $H$ commutes with every element of $N$. Hence

$$
F:N\times H\longrightarrow G,\qquad F(n,h)=nh
$$

is a [group homomorphism](../../../../../../../group-homomorphism.md), since $(n_1h_1)(n_2h_2)=n_1n_2h_1h_2$. Its [image of a group homomorphism](../../../../../../../image-of-a-group-homomorphism.md) is a [subgroup](../../../../../../../subgroup.md) containing both $N$ and $H$, and every product $nh$ lies in $\langle N,H\rangle$, so its image is exactly $\langle N,H\rangle$. If $nh=e$, then $n=h^{-1}\in N\cap H=\{e\}$, so $n=h=e$. Thus $F$ is injective and gives

$$
\boxed{\langle N,H\rangle\cong N\times H.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
