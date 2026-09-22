<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $B$ to be linear in its first argument and conjugate-linear in its second, with $\bar a=a^q$. For a [Hermitian form over a quadratic finite field](../../../../../../hermitian-form-over-a-quadratic-finite-field.md), $B(v,v)\in\mathbb F_q$. We first establish the [quadratic finite-field norm and trace surjectivity](../../../../../../quadratic-finite-field-norm-and-trace-surjectivity.md) needed for [orthonormalization of a finite-field Hermitian form](../../../../../../orthonormalization-of-a-finite-field-hermitian-form.md). The [field norm](../../../../../../field-norm.md) $N(a)=a^{q+1}$ maps $\mathbb F_{q^2}^*$ onto $\mathbb F_q^*$ because the [multiplicative group of a finite field is cyclic](../../../../../../multiplicative-group-of-a-finite-field-is-cyclic.md) of order $q^2-1$. The [field trace](../../../../../../field-trace.md) $\operatorname{Tr}(a)=a+a^q$ is an $\mathbb F_q$-linear map into $\mathbb F_q$. It is nonzero: a nonzero polynomial of degree $q$ cannot vanish at all $q^2$ elements. It is therefore onto, including in characteristic two.

There must be $v$ with $B(v,v)\ne0$. Otherwise, for any $v,w,a$, expanding the diagonal value gives

$$
0=B(v+aw,v+aw)=\operatorname{Tr}(\bar a B(v,w)).
$$

If $B(v,w)\ne0$, varying $a$ contradicts the surjectivity of the [field trace](../../../../../../field-trace.md). Thus all pairings would vanish, contrary to nondegeneracy. Choose $a$ with $N(a)=B(v,v)^{-1}$; then $v_1=av$ has norm one. Every $w$ decomposes uniquely as

$$
w=B(w,v_1)v_1+\bigl(w-B(w,v_1)v_1\bigr),\qquad V=\mathbb F_{q^2}v_1\oplus v_1^\perp.
$$

The restricted [Hermitian form over a quadratic finite field](../../../../../../hermitian-form-over-a-quadratic-finite-field.md) on the [orthogonal complement for a sesquilinear form](../../../../../../orthogonal-complement-for-a-sesquilinear-form.md) is nondegenerate: a vector there orthogonal to that complement is also orthogonal to $v_1$, hence to all of $V$, and is zero. Induction produces an [orthonormal basis](../../../../../../orthonormal-basis.md) $v_1,\ldots,v_n$.

The [unitary group over a finite field](../../../../../../unitary-group-over-a-finite-field.md) is the [group](../../../../../../group-split.md) of invertible $\mathbb F_{q^2}$-linear maps preserving $B$. In the [orthonormal basis](../../../../../../orthonormal-basis.md) just constructed, its concise description is

$$
\boxed{U_n(q^2)=\{g\in GL_n(\mathbb F_{q^2}):\bar g^{\mathsf T}g=I_n\}.}
$$

The notation here uses the size of the matrix field; it is also frequently written $U_n(q)$. There is no determinant-one condition in this definition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
