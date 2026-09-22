# Unit identities derived from the monoidal pentagon and triangle

↑ **Parent:** [Monoidal category](monoidal-category.md)

The [associator](associator.md) $a$ and [unitors](unitor.md) of a [monoidal category](monoidal-category.md) satisfy

$$
\rho_{X\otimes Y}=(1_X\otimes\rho_Y)a_{X,Y,I},\qquad
\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y,\qquad
\lambda_I=\rho_I.
$$

For the first identity, postcompose the pentagon on $X,Y,I,Z$ by $1_X\otimes(1_Y\otimes\lambda_Z)$, then use the triangle twice and cancel $a_{X,Y,Z}$. This gives the first equality after tensoring with $1_Z$; set $Z=I$ and cancel using the natural invertible right unitor. Reversing tensor order proves the second identity. Naturality of the left unitor at $\lambda_X$ gives $\lambda_{I\otimes X}=1_I\otimes\lambda_X$; comparing the second identity with the triangle on $I,I,X$ gives $(\lambda_I\otimes1_X)=(\rho_I\otimes1_X)$ and hence the last identity. These are consequences of the axioms, not extra axioms imported from the [monoidal coherence theorem](monoidal-coherence-theorem.md).

## ↑ Ancestors (6)

1. [Monoidal category](monoidal-category.md)
2. [Category theory](category-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25/6/solution.md)
- [Triangle identity for a monoidal category](triangle-identity-for-a-monoidal-category.md)
- [Word normalization proof of monoidal coherence](word-normalization-proof-of-monoidal-coherence.md)
