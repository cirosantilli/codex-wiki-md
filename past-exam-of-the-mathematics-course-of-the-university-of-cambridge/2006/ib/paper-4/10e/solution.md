<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

An [orthogonal transformation](../../../../../orthogonal-transformation.md) preserves the real [inner product](../../../../../inner-product.md). If $W$ is an [invariant subspace](../../../../../invariant-subspace.md), its orthogonal complement is invariant too: $\alpha W=W$ in finite dimensions, and for $v\in W^\perp$, $w\in W$, we have $\langle\alpha v,w\rangle=\langle v,\alpha^{-1}w\rangle=0$.

Complexify the space and the transformation. There is a complex [eigenvalue](../../../../../eigenvalue.md) $\lambda$, and preservation of the Hermitian norm gives $|\lambda|=1$. If $\lambda$ is real, it is $1$ or $-1$, and the real kernel of $\alpha-\lambda I$ contains a nonzero vector. Its span is an invariant line on which $\alpha$ acts as $+1$ or $-1$.

If $\lambda$ is nonreal, write an eigenvector as $u+iv$. Its real and imaginary parts are linearly independent: otherwise a nonzero real vector would have the nonreal eigenvalue. The real plane $W=\operatorname{span}(u,v)$ is invariant, because comparison of real and imaginary parts in $\alpha(u+iv)=\lambda(u+iv)$ gives real combinations of $u,v$. The restriction has determinant $\lambda\bar\lambda=1$. In an oriented orthonormal basis of $W$, it is therefore a rotation

$$
R_\theta=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.
$$

There is no invariant real line in this plane: such a line would supply a real eigenvalue, whereas its two eigenvalues are nonreal.

Apply the argument repeatedly to the invariant orthogonal complement. Thus **the smallest mutually orthogonal invariant blocks are lines with action $\pm1$, and planes with a genuine rotation**. Planes with angle $0$ or $\pi$ can be decomposed further into lines.

In dimension three a suitably chosen orthonormal basis therefore gives either

$$
\boxed{\operatorname{diag}(\epsilon_1,\epsilon_2,\epsilon_3),\quad \epsilon_j\in\{1,-1\},}
$$

or

$$
\boxed{\begin{pmatrix}\epsilon&0&0\\0&\cos\theta&-\sin\theta\\0&\sin\theta&\cos\theta\end{pmatrix},\quad\epsilon\in\{1,-1\},\quad0<\theta<\pi.}
$$

Changing the orientation of the plane reverses the angle, so this angle range loses no cases. These exhaust rotations, reflections and their possible compositions in three dimensions.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
