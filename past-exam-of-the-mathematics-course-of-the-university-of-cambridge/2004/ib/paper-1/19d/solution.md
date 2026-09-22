<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

The [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) are $[L_i,L_j]=i\hbar\epsilon_{ijk}L_k$. The [commutator](../../../../../commutator.md) product rule gives

$$
[L_i,L^2]=i\hbar\sum_{j,k}\epsilon_{ijk}(L_kL_j+L_jL_k)=0,
$$

since the bracketed expression is symmetric in $j,k$ and $\epsilon_{ijk}$ is antisymmetric. Also

$$
L_-L_+=L_1^2+L_2^2+i[L_1,L_2]=L_1^2+L_2^2-\hbar L_3,
$$

proving **$\boxed{L^2=L_-L_++L_3^2+\hbar L_3}$**.

For [orbital angular momentum](../../../../../orbital-angular-momentum.md), $L_i=-i\hbar\epsilon_{ijk}x_j\partial_k$. A differentiable radial function has $\partial_kf(r)=f'(r)x_k/r$, so its contraction with the antisymmetric symbol vanishes: $Lf(r)=0$. Put $s=x_1+ix_2$. The coordinate differential operators give $L_3s=\hbar s$, while

$$
L_+=\hbar\left[x_3(\partial_1+i\partial_2)-s\partial_3\right]
$$

annihilates every power of $s$, because $(\partial_1+i\partial_2)s=0$. Since all $L_i$ annihilate the radial factor, the product rule yields

$$
\boxed{L_3[s^nf(r)]=n\hbar s^nf(r),\qquad L_+[s^nf(r)]=0.}
$$

Substitution into the expression for $L^2$ gives the [highest-weight complex-coordinate orbital wavefunction](../../../../../highest-weight-complex-coordinate-orbital-wavefunction.md) result

$$
\boxed{L^2[s^nf(r)]=\hbar^2n(n+1)s^nf(r).}
$$

As $[L^2,L_-]=0$, lowering preserves this [eigenvalue](../../../../../eigenvalue.md) whenever the lowered function is nonzero. Explicitly,

$$
\boxed{L_-[s^nf(r)]=-2n\hbar x_3s^{n-1}f(r),\qquad
\text{unchanged eigenvalue }\hbar^2n(n+1).}
$$

For $n=0$ the lowered function is zero, so it is not an [eigenfunction](../../../../../eigenfunction.md). For $n\geq0$ the original nonzero function has the usual regular angular dependence. The PDF's “any integer” differential identities also hold locally for negative $n$ where $s\ne0$, but those negative powers are singular on the axis and are not square-integrable regular angular eigenstates. The converted TeX incorrectly writes $L_4$ in place of the PDF's $L_+$.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
