<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [algebra character](../../../../../../character-of-an-algebra.md) $\varphi$ is nonzero, linear and multiplicative, with $\varphi(1)=1$. Since $\varphi(a)\in\sigma_A(a)$, it satisfies $|\varphi(a)|\le\|a\|$ and is automatically continuous. If $h=h^*$ and $t\in\mathbb R$, then $(e^{ith})^*=e^{-ith}$, so $e^{ith}$ is a [Unitary element of a C-star algebra](../../../../../../unitary-element-of-a-c-star-algebra.md) and has [norm](../../../../../../norm.md) one. Hence

$$
|e^{it\varphi(h)}|=|\varphi(e^{ith})|\le1\qquad(t\in\mathbb R).
$$

Using both signs of $t$ forces $\operatorname{Im}\varphi(h)=0$. Write $x=h+ik$ with $h=(x+x^*)/2$ and $k=(x-x^*)/(2i)$ both [self-adjoint C-star elements](../../../../../../hermitian-element-of-a-c-star-algebra.md). Their [algebra character](../../../../../../character-of-an-algebra.md) values are real, and therefore

$$
\boxed{\varphi(x^*)=\overline{\varphi(x)}}.
$$

This is the conjugation in the original PDF; the converted TeX loses the bar.

For the final unheaded request, let $B=C^*(1,x)\subseteq A$. Normality makes this a commutative [unital](../../../../../../unital-algebra.md) [C-star subalgebra](../../../../../../c-star-subalgebra.md). We first justify spectral permanence, so that we do not silently use the possibly larger [algebra spectrum](../../../../../../spectrum-of-an-element.md) in a mere non-star subalgebra. A [self-adjoint C-star element](../../../../../../hermitian-element-of-a-c-star-algebra.md) $h$ in a [C-star algebra](../../../../../../c-star-algebra.md) has real [algebra spectrum](../../../../../../spectrum-of-an-element.md): $e^{ith}$ has [norm](../../../../../../norm.md) one, and $\lambda\in\sigma(h)$ implies $e^{it\lambda}\in\sigma(e^{ith})$ for each real $t$. The latter assertion follows from the factorization $e^{ith}-e^{it\lambda}1=(h-\lambda1)g_t(h)$ with commuting factors. An invertible product of commuting factors would make $h-\lambda1$ invertible. Both signs of $t$ then force $\lambda\in\mathbb R$.

A [compact](../../../../../../compact-space.md) subset of the real line has connected planar complement. Apply Question 1 to the [self-adjoint C-star element](../../../../../../hermitian-element-of-a-c-star-algebra.md) $h\in B$: all of $\rho_A(h)$ is its unbounded component and is retained in $B$. Thus $\sigma_A(h)=\sigma_B(h)$. If $a\in B$ is invertible in $A$, both $a^*a$ and $aa^*$ are [self-adjoint C-star elements](../../../../../../hermitian-element-of-a-c-star-algebra.md) and invertible in $A$, hence invertible in $B$. The elements $(a^*a)^{-1}a^*$ and $a^*(aa^*)^{-1}$ are respectively a left and a right inverse in $B$, so coincide and give its inverse. This proves [spectral permanence for C-star algebras](../../../../../../spectral-permanence-for-c-star-algebras.md).

In a commutative [unital](../../../../../../unital-algebra.md) complex [Banach algebra](../../../../../../banach-algebra-split.md), [algebra spectra](../../../../../../spectrum-of-an-element.md) are the ranges of the characters. Indeed a noninvertible $b-\lambda1$ lies in a [maximal ideal](../../../../../../maximal-ideal.md). Such an ideal is [closed](../../../../../../closed-set.md), since its proper closure cannot contain an element sufficiently near $1$. The quotient is a complex Banach division algebra; nonemptiness of the [algebra spectrum](../../../../../../spectrum-of-an-element.md) in that quotient makes each element scalar, producing an [algebra character](../../../../../../character-of-an-algebra.md) with value $\lambda$ at $b$. Conversely, an [algebra character](../../../../../../character-of-an-algebra.md) value cannot correspond to an invertible difference.

Apply this to $B$. The preceding involution result gives $\varphi(x^*)=\overline{\varphi(x)}$, and spectral permanence applies also to $p(x,x^*)$. Consequently

$$
\boxed{\sigma_A(p(x,x^*))=\{p(\lambda,\overline\lambda):\lambda\in\sigma_A(x)\}}.
$$

Thus the second argument is conjugated as in the original PDF, not a second copy of $\lambda$. This is the spectral mapping rule for a [star polynomial in one normal element](../../../../../../star-polynomial-in-one-normal-element.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
