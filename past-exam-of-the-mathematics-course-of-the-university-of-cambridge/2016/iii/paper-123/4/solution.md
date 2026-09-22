<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $K=\mathbb Q(\sqrt{-31})$. Its [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) is $\mathbb Z[(1+\sqrt{-31})/2]$, and its fundamental [field discriminant](../../../../../field-discriminant.md) is $-31$.

First compute the [class number](../../../../../class-number.md). The [ideal-form correspondence for imaginary quadratic fields](../../../../../ideal-form-correspondence-for-imaginary-quadratic-fields.md) identifies the ideal classes with proper equivalence classes of primitive positive definite [binary quadratic forms](../../../../../binary-quadratic-form.md) of discriminant $-31$. Each has a unique [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) representative under the convention $|b|\leq a\leq c$, with $b\geq0$ when $|b|=a$ or $a=c$. From $31=4ac-b^2\geq3a^2$ we get $1\leq a\leq\sqrt{31/3}<4$. Checking these three possible leading coefficients gives exactly

$$
[1,1,8],\qquad[2,1,4],\qquad[2,-1,4].
$$

For $a=3$, neither odd residue choice $b=\pm1,\pm3$ makes $(b^2+31)/12$ integral. The listed forms are primitive and satisfy the reduction convention, so

$$
\boxed{h_K=3,\qquad\operatorname{Cl}(K)\cong C_3.}
$$

This computes the [ideal class group of Q of square root minus thirty-one](../../../../../ideal-class-group-of-q-of-square-root-minus-thirty-one.md).

Now take a root $\theta$ of $F(T)=T^3+T-1$, and let $H$ be its splitting field over $\mathbb Q$. There is no rational root: the only candidates are $\pm1$, and neither vanishes. Thus the cubic is irreducible. Its [polynomial discriminant](../../../../../polynomial-discriminant.md) is

$$
\operatorname{disc}(F)=-4-27=-31.
$$

Since this is nonsquare, the [Galois group of an irreducible cubic](../../../../../galois-group-of-an-irreducible-cubic.md) is $S_3$. Its quadratic subfield is $K$: the product of pairwise root differences squares to $-31$ and changes sign under odd permutations. Thus $H/K$ is cyclic of degree three, and $H=K(\theta)$. Indeed the cubic field and $K$ have coprime degrees, so their compositum already has the full splitting-field degree six. The squarefree [polynomial discriminant](../../../../../polynomial-discriminant.md) also shows, by the [discriminant-index formula for an integral lattice](../../../../../discriminant-index-formula-for-an-integral-lattice.md), that $\mathbb Z[\theta]$ is the full integer ring of the cubic field.

It remains to prove that $H/K$ is unramified everywhere. At any rational prime $\ell\ne31$, the reduction of $F$ is separable. Over a finite residue extension in which it splits, all residue roots are simple and lift by [Hensel lemma](../../../../../hensel-s-lemma.md) to the corresponding [unramified extension](../../../../../unramified-extension.md) of $\mathbb Q_\ell$. Therefore the local splitting field is unramified over $\mathbb Q_\ell$, and its extension over a completion of $K$ is unramified as well.

At the only possible ramified prime, direct reduction gives

$$
F(T)\equiv(T-17)^2(T-28)\pmod{31},\qquad F'(28)\equiv28\not\equiv0\pmod{31}.
$$

The simple root lifts to $r\in\mathbb Q_{31}$. Write $F(T)=(T-r)Q(T)$, with $Q$ monic quadratic over $\mathbb Q_{31}$. The discriminant product formula gives

$$
\operatorname{disc}(F)=\operatorname{disc}(Q)\,Q(r)^2.
$$

Here $Q(r)=F'(r)$ is a unit, so the [quadratic discriminant](../../../../../quadratic-discriminant.md) has square class $-31$. Hence the entire local splitting field is

$$
\mathbb Q_{31}(\sqrt{\operatorname{disc}(Q)})=\mathbb Q_{31}(\sqrt{-31})=K_{31}.
$$

It is quadratic over $\mathbb Q_{31}$, but its extension over the completion of $K$ is trivial. Thus the prime over $31$ splits completely in $H/K$; in particular it is not ramified there. This is the local splitting-field argument behind an [unramified cyclic cubic extension from a prime-discriminant cubic](../../../../../unramified-cyclic-cubic-extension-from-a-prime-discriminant-cubic.md). There are no real places of the imaginary quadratic field $K$, so no infinite-place ramification remains to check.

The [Hilbert class field](../../../../../hilbert-class-field.md) theorem identifies the maximal everywhere unramified abelian extension with an extension of degree $h_K$. Our cyclic [unramified extension](../../../../../unramified-extension.md) already has that degree, so it must be the whole [Hilbert class field](../../../../../hilbert-class-field.md). Therefore

$$
\boxed{H_K=\mathbb Q(\sqrt{-31},\theta),\qquad\theta^3+\theta-1=0.}
$$

Equivalently, it is the splitting field of $T^3+T-1$, of degree six over $\mathbb Q$ and degree three over $K$. Replacing $\theta$ by $\theta^{-1}$ gives the alternative defining cubic $T^3-T^2-1$. This is the [Hilbert class field of Q of square root minus thirty-one](../../../../../hilbert-class-field-of-q-of-square-root-minus-thirty-one.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 123](../../paper-123-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
