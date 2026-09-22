<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is no infinite component in the modulus $(5)$. The ordinary [ideal class group](../../../../../../ideal-class-group.md) of $\mathbb Q$ is trivial, and its [unit group](../../../../../../unit-group.md) is $\{\pm1\}$. The [ray class exact sequence](../../../../../../ray-class-exact-sequence.md) therefore gives

$$
\boxed{\operatorname{Cl}_{(5)}(\mathbb Q)
\simeq(\mathbb Z/5\mathbb Z)^\times/\{\pm1\}\simeq C_2.}
$$

Concretely, a [fractional ideal](../../../../../../fractional-ideal.md) prime to $5$ has a rational generator $r=a/b$ with $5\nmid ab$. Reducing $r$ modulo $5$ is well-defined up to multiplication by the units $\pm1$. Its ray class is trivial precisely when one of the two generators $r,-r$ is congruent to one. Thus the quotient has the two classes $\{1,4\}$ and $\{2,3\}$. No positivity restriction is imposed on a generator.

To identify the corresponding field, put $E=\mathbb Q(\zeta_5+\zeta_5^{-1})=\mathbb Q(\sqrt5)$. The [maximal real subfield of the fifth cyclotomic field](../../../../../../maximal-real-subfield-of-the-fifth-cyclotomic-field.md) is fixed by complex conjugation, the element $-1$ of $(\mathbb Z/5\mathbb Z)^\times$. For a prime $\ell\ne5$, the [Frobenius automorphism](../../../../../../frobenius-automorphism.md) of $\mathbb Q(\zeta_5)/\mathbb Q$ is $\zeta_5\mapsto\zeta_5^\ell$. Its restriction to $E$ thus corresponds exactly to the residue class of $\ell$ modulo $\{\pm1\}$. Multiplicativity extends this to the [Artin reciprocity map](../../../../../../artin-reciprocity-law.md) on all [fractional ideals](../../../../../../fractional-ideal.md) prime to $5$, whose kernel is exactly $P_{\mathbb Q,1}((5))$. Its [field discriminant](../../../../../../field-discriminant.md) $5$ also confirms that $E$ is [unramified](../../../../../../unramified-extension.md) outside $5$; moreover $E$ is a [totally real number field](../../../../../../totally-real-number-field.md). The uniqueness in the [Main theorem of class field theory](../../../../../../main-theorem-of-class-field-theory.md) now gives

$$
\boxed{\mathbb Q_{(5)}=\mathbb Q(\sqrt5).}
$$

Including the real place changes the [ray class group](../../../../../../ray-class-group.md): a principal generator must then be positive as well as congruent to one. The [residue and signature group of a modulus](../../../../../../residue-and-signature-group-of-a-modulus.md) gives

$$
\operatorname{Cl}_{(5)\infty}(\mathbb Q)
\simeq\bigl((\mathbb Z/5\mathbb Z)^\times\times\{\pm1\}\bigr)
/\langle(-1,-1)\rangle
\simeq(\mathbb Z/5\mathbb Z)^\times.
$$

Here the isomorphism sends $(u,\varepsilon)$ to $\varepsilon u$. Consequently $\mathbb Q_{(5)\infty}=\mathbb Q(\zeta_5)$, of degree four. **The finite modulus gives the real quadratic field; the modulus with the real place gives the full cyclotomic field.** The printed finite-modulus assertion needs no correction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
