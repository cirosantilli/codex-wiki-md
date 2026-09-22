<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

A [group homomorphism](../../../../../group-homomorphism.md) sends identity to identity. For $\theta(g),\theta(h)$ in its image,

$$
\theta(g)\theta(h)^{-1}=\theta(gh^{-1}),
$$

which is still in the image; hence the [image of a group homomorphism](../../../../../image-of-a-group-homomorphism.md) is a [subgroup](../../../../../subgroup.md) of $H$. Let $N=\ker\theta$. It is a [subgroup](../../../../../subgroup.md) by the same identity, and for $k\in N$ and $g\in G$,

$$
\theta(gkg^{-1})=\theta(g)\theta(k)\theta(g)^{-1}=e.
$$

Thus $gNg^{-1}\subseteq N$, and replacing $g$ by $g^{-1}$ gives equality, proving that $N$ is a [normal subgroup](../../../../../normal-subgroup.md).

Define a map from the [quotient group](../../../../../quotient-group.md) by

$$
\Phi:G/N\longrightarrow\theta(G),\qquad \Phi(gN)=\theta(g).
$$

If $gN=hN$, then $h^{-1}g\in N$ and $\theta(g)=\theta(h)$, so the map is well defined. Conversely equality of the images implies $h^{-1}g\in N$, giving injectivity. It is onto by the definition of image, and $\Phi((gN)(hN))=\theta(gh)=\theta(g)\theta(h)$. This proves the [first isomorphism theorem for groups](../../../../../first-isomorphism-theorem.md) in this case:

$$
\boxed{G/\ker\theta\cong\theta(G)}.
$$

An [orthogonal matrix](../../../../../orthogonal-matrix.md) $Q$ has $Q^{\mathsf T}Q=I$, so $(\det Q)^2=1$. The [determinant](../../../../../determinant.md) is therefore a [group homomorphism](../../../../../group-homomorphism.md) $O(3)\to\{1,-1\}$, with image both signs because $\operatorname{diag}(-1,1,1)$ has determinant $-1$. Its kernel is the [special orthogonal group](../../../../../special-orthogonal-group.md) $SO(3)$. Hence **$SO(3)$ is normal in $O(3)$**, and

$$
\boxed{O(3)/SO(3)\cong\{1,-1\}\cong C_2}.
$$

For the last request, the [determinant-twist projection in odd dimension](../../../../../determinant-twist-projection-in-odd-dimension.md) gives an explicit example:

$$
\boxed{\pi:O(3)\longrightarrow SO(3),\qquad \pi(Q)=(\det Q)Q}.
$$

Indeed $\det\pi(Q)=(\det Q)^4=1$, and scalar factors commute, so $\pi(QR)=\pi(Q)\pi(R)$. If $\pi(Q)=I$, then $Q=(\det Q)I$, making $Q=I$ or $Q=-I$. Both lie in the kernel, which is therefore exactly $\{I,-I\}$, of order two. The map also fixes every member of $SO(3)$, so it is onto.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
