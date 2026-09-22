# Symplectic Gram-Schmidt process

↑ **Parent:** [Symplectic basis](symplectic-basis.md)

Construct a [symplectic basis](symplectic-basis.md) two [vectors](vector.md) at a time. Choose $e\ne0$; the [nondegenerate bilinear form](nondegenerate-bilinear-form.md) supplies $g$ with $\omega(e,g)\ne0$, and set $f=g/\omega(e,g)$. For any [vector](vector.md) $x$, remove its paired components by

$$
x'=x-\omega(x,f)e+\omega(x,e)f.
$$

Then $\omega(x',e)=\omega(x',f)=0$. Thus, for $U=\operatorname{span}\{e,f\}$, the [symplectic orthogonal complement](symplectic-orthogonal-complement.md) gives a [direct sum](direct-sum.md) $V=U\oplus U^\omega$; its restricted [bilinear form](bilinear-form.md) remains [nondegenerate](nondegenerate-bilinear-form.md). Repeat there until no [vectors](vector.md) remain, then put all $e_i$ before all $f_i$. This proves even [dimension](dimension-vector-space.md) and existence together. Only the nonzero pairing is divided out, so the construction also works in [characteristic](characteristic-of-a-field.md) two. The pair-splitting argument is described in [Bilinear Forms by Keith Conrad](bilinear-forms-by-keith-conrad.md) (Keith Conrad, Bilinear Forms, §5, proof of Theorem 5.1 and Theorem 5.4).

## ↑ Ancestors (9)

1. [Symplectic basis](symplectic-basis.md)
2. [Symplectic vector space](symplectic-vector-space.md)
3. [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
4. [Bilinear form](bilinear-form.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
