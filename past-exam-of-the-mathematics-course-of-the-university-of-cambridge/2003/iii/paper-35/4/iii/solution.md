<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**True: quantum entropy is subadditive.** Write $\sigma=\rho_1\otimes\rho_2$. Positivity ensures the support of $\rho$ lies in that of $\sigma$. Indeed, if $|v\rangle\in\ker\rho_1$, then $\sum_j\langle v,j|\rho|v,j\rangle=0$; all summands are nonnegative, so $\rho^{1/2}|v,j\rangle=0$ for every $j$. Thus $\rho$ annihilates $\ker\rho_1\otimes\mathcal K_2$, and similarly the kernel from the other factor.

On the resulting support, $\log_2(\rho_1\otimes\rho_2)=\log_2\rho_1\otimes I+I\otimes\log_2\rho_2$. Using the defining property of the [partial trace](../../../../../../partial-trace.md) and [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) proved in part (i),

$$
0\le D(\rho\|\rho_1\otimes\rho_2)
=-S(\rho)-\operatorname{tr}\rho_1\log_2\rho_1-\operatorname{tr}\rho_2\log_2\rho_2
=S(\rho_1)+S(\rho_2)-S(\rho).
$$

Hence

$$
\boxed{S(\rho)\le S(\rho_1)+S(\rho_2).}
$$

Equality holds exactly for the [product state](../../../../../../product-state.md) $\rho=\rho_1\otimes\rho_2$. This proves [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) directly.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
