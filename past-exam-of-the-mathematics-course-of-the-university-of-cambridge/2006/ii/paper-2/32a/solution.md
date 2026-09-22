<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

With $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$, the matrix of $S_z\cos\theta+S_x\sin\theta$ is $(\hbar/2)\begin{pmatrix}\cos\theta&\sin\theta\\\sin\theta&-\cos\theta\end{pmatrix}$. Multiplication by $(c,s)^T$ and $(-s,c)^T$ gives [eigenvalues](../../../../../eigenvalue.md) $+\hbar/2$ and $-\hbar/2$, using the double-angle identities.

The one-particle transformation is the matrix $R=\begin{pmatrix}c&-s\\s&c\end{pmatrix}$, with [determinant](../../../../../determinant.md) one. The antisymmetric tensor $|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle$ transforms by this [determinant](../../../../../determinant.md) under $R\otimes R$, so the singlet is unchanged. The total $S_z$ kills it. Its invariance under these rotations implies that total $S_z\cos\theta+S_x\sin\theta$ also kills it for every $\theta$, so total $S_x$ kills it. The spin commutator then gives total $S_y$ acting as zero. Therefore **$S^2|\chi\rangle=0$** and it has total spin zero.

Rotating only particle B produces

$$
|\chi_\theta\rangle=\frac1{\sqrt2}(-s|\uparrow\uparrow\rangle+c|\uparrow\downarrow\rangle-c|\downarrow\uparrow\rangle-s|\downarrow\downarrow\rangle).
$$

The measurement [probabilities](../../../../../probability.md) are therefore

$$
\boxed{P(\uparrow,\uparrow)=P(\downarrow,\downarrow)=\tfrac12\sin^2(\theta/2),\qquad P(\uparrow,\downarrow)=P(\downarrow,\uparrow)=\tfrac12\cos^2(\theta/2).}
$$

Each arrow represents the corresponding value $\pm\hbar/2$. The sequential measurements commute because they act on different particles. The two parallel outcomes leave [triplet states](../../../../../spin-one-half-triplet-state.md) with total spin one and **$S^2=2\hbar^2$**. Each antiparallel [product state](../../../../../product-state.md) is a superposition of the spin-zero singlet and the spin-one zero-projection triplet, and is not an $S^2$ eigenstate. Outcomes of zero [probability](../../../../../probability.md) at a special angle do not actually occur.

## ↑ Ancestors (10)

1. [32A](../32a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
