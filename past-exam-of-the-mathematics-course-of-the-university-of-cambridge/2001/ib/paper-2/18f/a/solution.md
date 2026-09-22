<h1 id="18f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [orbital angular momentum](../../../../../../orbital-angular-momentum.md) operators are

$$
\boxed{L_1=x_2p_3-x_3p_2,\qquad L_2=x_3p_1-x_1p_3,\qquad L_3=x_1p_2-x_2p_1.}
$$

On smooth wavefunctions, $[x_i,p_j]=i\hbar\delta_{ij}$, while position operators commute with each other and momentum operators commute with each other. Applying the product rule for [commutators](../../../../../../commutator.md) gives

$$
[x_ip_j,x_kp_l]=-i\hbar\delta_{jk}x_ip_l+i\hbar\delta_{il}x_kp_j.
$$

Use it on the four terms in $[L_1,L_2]$: only $[x_2p_3,x_3p_1]=-i\hbar x_2p_1$ and $[x_3p_2,x_1p_3]=i\hbar x_1p_2$ survive, with the latter entering positively from the two minus signs. Therefore

$$
\boxed{[L_1,L_2]=i\hbar L_3.}
$$

The cyclic versions similarly give $[L_3,L_1]=i\hbar L_2$ and $[L_3,L_2]=-i\hbar L_1$. Thus, for $L_\pm=L_1\pm iL_2$,

$$
\boxed{[L_3,L_\pm]=\pm\hbar L_\pm.}
$$

Now define $L^2=L_1^2+L_2^2+L_3^2$. For each $i$,

$$
[L^2,L_i]=i\hbar\sum_{j,k}\epsilon_{jik}(L_jL_k+L_kL_j)=0,
$$

because the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) is antisymmetric in $j,k$ and the operator pair is symmetric. Linearity then gives **$\boxed{[L^2,L_\pm]=0}$**. The PDF superscript here is the squared total angular momentum, not the component $L_2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18F](../../18f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
