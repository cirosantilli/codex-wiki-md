<h1 id="18f/solution">Solution</h1>

↑ **Parent:** [18F](../18f.md)

An automorphism sends the [primitive root of unity](../../../../../primitive-root-of-unity.md) $\xi_n$ to another [primitive root of unity](../../../../../primitive-root-of-unity.md), hence uniquely to $\xi_n^a$ with $a\in(\mathbb Z/n\mathbb Z)^*$. Define $\chi(\sigma)=a$. Composition multiplies exponents, and an automorphism with exponent one fixes the generator and thus all of $L$. Therefore **$\chi$ is an injective group homomorphism** and $G$ is abelian.

The extension is finite Galois: it is the [splitting field](../../../../../splitting-field.md) of $X^n-1$, whose roots are all present and distinct. Existence of a root of order $n$ in positive characteristic implies that the characteristic does not divide $n$. The [Fundamental theorem of Galois theory](../../../../../fundamental-theorem-of-galois-theory.md) identifies an intermediate field with $L^H$. Since $G$ is abelian, $H$ is normal; the normal-subgroup criterion gives **$L^H/K$ Galois**, with group $G/H$.

For a non-surjective nontrivial example, take $K=\mathbb Q(i)$ and $n=8$. Its cyclotomic extension has degree two, and its image is $\{1,5\}$ inside the four-element group $(\mathbb Z/8\mathbb Z)^*$. For $K=\mathbb Q$ and prime $p$, $\Phi_p(X)=1+\cdots+X^{p-1}$ is irreducible: $\Phi_p(X+1)$ is Eisenstein at $p$. Thus the extension has degree $p-1$, equal to the [unit group](../../../../../unit-group.md)'s order, proving surjectivity.

For $n=7$, let $\zeta=\xi_7$. The cyclic [Galois group](../../../../../galois-group.md) of order six has exactly one subgroup of each order dividing six, so there are exactly four fields:

$$
\begin{array}{c|c}
M&\operatorname{Aut}(\mathbb Q(\zeta)/M)\\\hline
\mathbb Q&\{\sigma_a:a=1,2,3,4,5,6\}\\
\mathbb Q(\sqrt{-7})&\{\sigma_1,\sigma_2,\sigma_4\}\\
\mathbb Q(\zeta+\zeta^{-1})&\{\sigma_1,\sigma_6\}\\
\mathbb Q(\zeta)&\{\sigma_1\}
\end{array}
$$

Here $\sigma_a(\zeta)=\zeta^a$. To identify the quadratic field without guessing, put $A=\zeta+\zeta^2+\zeta^4$ and $B=\zeta^3+\zeta^5+\zeta^6$. Multiplication gives $A+B=-1$ and $AB=2$, so $(A-B)^2=-7$. The order-three subgroup fixes $A$, and $A-B\notin\mathbb Q$, proving the quadratic identification. The real field is cubic because complex conjugation is $\sigma_6$, with fixed subgroup of order two.

## ↑ Ancestors (10)

1. [18F](../18f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
