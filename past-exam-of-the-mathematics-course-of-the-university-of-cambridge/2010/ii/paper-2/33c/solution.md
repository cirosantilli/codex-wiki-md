<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

The rotation [unitary operator](../../../../../unitary-operator.md) is **$U(\mathbf n,\theta)=\exp(-i\theta\,\mathbf n\cdot\mathbf J/\hbar)$.** A state with zero [orbital angular momentum](../../../../../orbital-angular-momentum.md) has a rotationally invariant orbital factor; a spinless $j=0$ state is wholly unchanged. Zero orbital angular momentum alone does not rule out a nontrivial rotation of intrinsic [spin angular momentum](../../../../../spin.md).

For [spin one-half](../../../../../spin-one-half.md), $\mathbf J=\hbar\boldsymbol\sigma/2$. Direct multiplication of the [Pauli matrices](../../../../../pauli-matrices.md) gives $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$. The antisymmetric part vanishes when contracted with $a_ia_j$, hence

$$
\boxed{(\mathbf J\cdot\mathbf a)^2=\frac{\hbar^2|\mathbf a|^2}{4}I}.
$$

For $\mathbf a\ne0$, the operator has trace zero, so its [eigenvalues](../../../../../eigenvalue.md) are $\pm\hbar|\mathbf a|/2$; for $\mathbf a=0$ both are zero. With unit $\mathbf n$, the even and odd powers in the exponential give

$$
U(\mathbf n,\theta)=I\cos(\theta/2)-i\,\mathbf n\cdot\boldsymbol\sigma\sin(\theta/2).
$$

Take $\mathbf n'=(\sin\theta,0,\cos\theta)$. The rotated state $|m'\rangle_\theta=U(\mathbf y,\theta)|m'\rangle$ satisfies **$(\mathbf n'\cdot\mathbf J)|m'\rangle_\theta=m'\hbar|m'\rangle_\theta$**, because $U J_3U^\dagger=\mathbf n'\cdot\mathbf J$. By the [Born rule](../../../../../born-rule.md), the probability of this outcome in the initial state $|m\rangle$ is $|{}_\theta\langle m'|m\rangle|^2=|\langle m|U(\mathbf y,\theta)|m'\rangle|^2$. In the $J_3$ eigenbasis,

$$
U(\mathbf y,\theta)=\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}.
$$

The transition from $m=1/2$ to $m'=-1/2$ thus has probability $\sin^2(\theta/2)=1-\cos^2(\theta/2)$. **$\boxed{A=1,\quad B=-1}$.**

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
