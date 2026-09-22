<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In this part identify $\mathbb T$ with the [complex unit circle](../../../../../../complex-unit-circle.md) by $t\mapsto e^{it}$. Write the finite [abelian group](../../../../../../abelian-group.md) $G$ additively and let $\widehat G=\operatorname{Hom}(G,\mathbb T)$, with pointwise multiplication, be the [character group of a finite abelian group](../../../../../../character-group-of-a-finite-abelian-group.md) of $G$. A [linear character](../../../../../../linear-character.md) has modulus one, since its values have finite order. We first prove the extension and counting facts needed for [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md).

If $H\le G$, $\chi\in\widehat H$, and $x\notin H$, let $d$ be the least positive integer with $dx\in H$. Choose $z\in\mathbb T$ with $z^d=\chi(dx)$ and define

$$
\widetilde\chi(h+jx)=\chi(h)z^j.
$$

This is well-defined: two representations differ by $j-j'=qd$ and $h-h'=-qdx$, whose contributions cancel. It is a [group homomorphism](../../../../../../group-homomorphism.md) and extends $\chi$. Conversely every extension has this form, and the equation for $z$ has exactly $d$ distinct roots. Since $[H+\langle x\rangle:H]=d$, successive adjunctions prove that each [linear character](../../../../../../linear-character.md) of $H$ has exactly $[G:H]$ extensions. Taking $H=\{0\}$ gives $\boxed{|\widehat G|=|G|}$. This is the [extension of a character across a cyclic quotient](../../../../../../extension-of-a-character-across-a-cyclic-quotient.md), proved here without a structure theorem. Extending the [linear character](../../../../../../linear-character.md) sending a nonzero element $g$ of order $d$ to $e^{2\pi i/d}$ also proves that [linear characters](../../../../../../linear-character.md) separate points of $G$.

Use the normalized [inner product](../../../../../../inner-product.md) $\langle f,g\rangle=|G|^{-1}\sum_{x\in G}f(x)\overline{g(x)}$. For a nontrivial [linear character](../../../../../../linear-character.md) $\chi$, choose $a$ with $\chi(a)\ne1$. Translation of the sum gives $\sum_x\chi(x)=\chi(a)\sum_x\chi(x)$, so that sum is zero. Applying this to $\chi\overline\psi$ gives

$$
\boxed{\langle\chi,\psi\rangle=\mathbf1_{\{\chi=\psi\}}.}
$$

There are $|G|$ such orthonormal vectors in the $|G|$-dimensional space $\mathbb C^G$, so they form an [orthonormal basis](../../../../../../orthonormal-basis.md). Define the [Fourier coefficients](../../../../../../fourier-coefficient.md) by $\widehat f(\chi)=|G|^{-1}\sum_x f(x)\overline{\chi(x)}$. Expanding in that basis proves [Fourier inversion on a finite group](../../../../../../fourier-inversion-on-a-finite-group.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md):

$$
\boxed{f(x)=\sum_{\chi\in\widehat G}\widehat f(\chi)\chi(x),\qquad
\langle f,g\rangle=\sum_{\chi\in\widehat G}\widehat f(\chi)\overline{\widehat g(\chi)}.}
$$

For normalized [convolution](../../../../../../convolution.md) $(f*g)(x)=|G|^{-1}\sum_y f(y)g(x-y)$, changing the finite summation variables yields $\widehat{f*g}(\chi)=\widehat f(\chi)\widehat g(\chi)$. Translation $f(x)\mapsto f(x+a)$ multiplies its [Fourier coefficient](../../../../../../fourier-coefficient.md) by $\chi(a)$. These formulas fix all normalization and conjugation conventions.

The PDF's double-hat identification is canonical [Pontryagin duality](../../../../../../pontryagin-duality.md): define $e:G\to\widehat{\widehat G}$ by $e_x(\chi)=\chi(x)$. This is a [group homomorphism](../../../../../../group-homomorphism.md) and is injective because [linear characters](../../../../../../linear-character.md) separate points. Applying the already proved character-counting result to $\widehat G$ shows that both groups have size $|G|$, so

$$
\boxed{G\cong\widehat{\widehat G}\quad\text{canonically by evaluation}.}
$$

The TeX loses one hat. For completeness, the single-dual isomorphism $\widehat G\cong G$ also holds, but is generally noncanonical. Here is a proof including the needed finite cyclic decomposition. Choose an element $a$ of maximal order $d$. Every element order divides $d$: for two elements, extract their prime-power components by integer multiples: if an element has order $d$ and $p^\alpha$ is the exact power of $p$ in $d$, multiplying it by $d/p^\alpha$ gives order $p^\alpha$. Then combine the components with the larger order for each prime. Components of coprime orders have a sum of product order, because their [cyclic subgroups](../../../../../../cyclic-subgroup.md) have trivial intersection. This constructs an element of order the [least common multiple](../../../../../../least-common-multiple.md) of the two original orders, which cannot exceed maximal $d$; hence each order divides $d$.

Extend the primitive [linear character](../../../../../../linear-character.md) of $\langle a\rangle$ to $\chi:G\to\mathbb T$. All its values are $d$th roots because all element orders divide $d$. Define $\rho(g)=ja$ when $\chi(g)=e^{2\pi ij/d}$. This is a [group homomorphism](../../../../../../group-homomorphism.md) fixing $\langle a\rangle$, and $g=\rho(g)+(g-\rho(g))$ shows $G=\langle a\rangle\oplus\ker\rho$. Induction on group size decomposes $G$ into finite [cyclic groups](../../../../../../cyclic-group.md). A [cyclic group](../../../../../../cyclic-group.md) of order $d_j$ has precisely the [linear characters](../../../../../../linear-character.md) $j\mapsto e^{2\pi imj/d_j}$ and hence a [character group of a finite abelian group](../../../../../../character-group-of-a-finite-abelian-group.md) isomorphic to itself. The dual of a finite [direct product of groups](../../../../../../direct-product-of-groups.md) is the product of its factor duals, since a [linear character](../../../../../../linear-character.md) is determined by its restrictions. This proves $\widehat G\cong G$ after choices of cyclic factors and generators, without using an unproved finite-abelian-group structure theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
