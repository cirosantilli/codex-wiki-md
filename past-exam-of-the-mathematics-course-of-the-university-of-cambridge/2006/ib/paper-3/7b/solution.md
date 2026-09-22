<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

In the position representation, $\hat p=-i\hbar\nabla$. The [orbital angular momentum](../../../../../orbital-angular-momentum.md) operator and its squared magnitude are

$$
\boxed{\hat L=\hat x\times\hat p=-i\hbar\hat x\times\nabla,\qquad
\hat L^2=\sum_{i=1}^3\hat L_i^2.}
$$

For example, with $D=x\cdot\nabla$, the latter is $-\hbar^2[r^2\Delta-D^2-D]$. Operator products here act on smooth [wavefunctions](../../../../../wave-function.md) in a common invariant domain.

To calculate the [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md), use $[x_a,p_b]=i\hbar\delta_{ab}$ and the vanishing position-position and momentum-momentum [commutators](../../../../../commutator.md). Expanding the products gives

$$
[x_ap_b,x_cp_d]=i\hbar(\delta_{ad}x_cp_b-\delta_{bc}x_ap_d).
$$

Multiplication by $\epsilon_{iab}\epsilon_{jcd}$ then gives

$$
\begin{aligned}
[L_i,L_j]
&=i\hbar\epsilon_{iab}\epsilon_{jcd}
(\delta_{ad}x_cp_b-\delta_{bc}x_ap_d)\\
&=i\hbar(x_i p_j-x_j p_i)
=i\hbar\epsilon_{ijk}L_k.
\end{aligned}
$$

Finally, the product commutator rule yields

$$
[L^2,L_i]=\sum_j\bigl(L_j[L_j,L_i]+[L_j,L_i]L_j\bigr)
=i\hbar\sum_{j,k}\epsilon_{jik}(L_jL_k+L_kL_j)=0.
$$

The final cancellation pairs the antisymmetric [Levi-Civita symbol](../../../../../levi-civita-symbol.md) with an expression symmetric in $j,k$. Thus

$$
\boxed{[L_i,L_j]=i\hbar\epsilon_{ijk}L_k,\qquad [L^2,L_i]=0.}
$$

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
