<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [algebra involution](../../../../../algebra-involution.md) is a map $x\mapsto x^*$ satisfying

$$
(\alpha x+\beta y)^*=\overline\alpha x^*+\overline\beta y^*,\qquad
(xy)^*=y^*x^*,\qquad (x^*)^*=x.
$$

Thus it is a [conjugate-linear map](../../../../../antilinear-map.md), reverses multiplication, and has square equal to the identity map. These are algebraic axioms; [norm](../../../../../norm.md) [continuity](../../../../../continuous-function.md), when included in a convention for a Banach star algebra, is an additional requirement and is not used here. A [Hermitian element of a star algebra](../../../../../hermitian-element-of-a-star-algebra.md) satisfies $h^*=h$.

Conjugate [linearity](../../../../../linearity.md) gives $0^*=0$. The map $*$ is surjective, so every $u$ is $v^*$ for some $v$. The identities $(v1)^*=1^*v^*=v^*$ and $(1v)^*=v^*1^*=v^*$ show that $1^*$ is a two-sided identity; uniqueness of the identity gives $1^*=1$. Therefore **both zero and the identity are [Hermitian algebra elements](../../../../../hermitian-element-of-a-star-algebra.md)**.

For the final unheaded request, first prove equality of the two spectra for a [Hermitian element of a star algebra](../../../../../hermitian-element-of-a-star-algebra.md) $h\in B$. Write $D=\mathbb C\setminus\sigma_A(h)$. The spectrum is a [compact](../../../../../compact-space.md) subset of the real axis by the assumption that $A$ is a [Hermitian Banach algebra](../../../../../hermitian-banach-algebra.md), so $D$ is [connected](../../../../../connected-space.md): points above and below the real axis can be joined by paths passing beyond the endpoints of an interval containing the spectrum; points of the real axis outside the spectrum can first move a short distance vertically. Define

$$
E=\{\lambda\in D:(\lambda1-h)^{-1}\in B\}.
$$

For large $|\lambda|$, the [Neumann series](../../../../../neumann-series.md) $\lambda^{-1}\sum_{n\ge0}(h/\lambda)^n$ converges in the [closed](../../../../../closed-set.md) unital [star-subalgebra](../../../../../star-subalgebra.md) $B$, so $E$ is nonempty. It is relatively open in $D$ by the same series applied to a perturbation of an already invertible element of $B$. It is relatively [closed](../../../../../closed-set.md) in $D$, since the [resolvent of an element](../../../../../resolvent-of-an-element.md) is [continuous](../../../../../continuous-function.md) in $A$ and $B$ is [closed](../../../../../closed-set.md). Connectedness gives $E=D$. Conversely an inverse in $B$ is an inverse in $A$, so

$$
\sigma_B(h)=\sigma_A(h).
$$

This proves the needed [spectrum in a closed unital subalgebra](../../../../../spectrum-in-a-closed-unital-subalgebra.md) equality for [Hermitian algebra elements](../../../../../hermitian-element-of-a-star-algebra.md) without presupposing that their spectra in $B$ are real.

Now suppose $b\in B$ is invertible in $A$. Both $bb^*$ and $b^*b$ are [Hermitian algebra elements](../../../../../hermitian-element-of-a-star-algebra.md), since reversing products and applying $*$ twice fixes them. They are invertible in $A$, by part (ii), so the preceding equality of spectra of [Hermitian algebra elements](../../../../../hermitian-element-of-a-star-algebra.md) makes them invertible in $B$. Part (ii), applied within $B$, then makes $b$ invertible in $B$. Applying this to $b-\lambda1$ for every scalar $\lambda$, and using the automatic converse for an inverse already in $B$, proves [spectral permanence for Hermitian Banach algebras](../../../../../spectral-permanence-for-hermitian-banach-algebras.md):

$$
\boxed{\sigma_B(b)=\sigma_A(b)\quad(b\in B).}
$$

Only closedness, a common identity, closure under the [algebra involution](../../../../../algebra-involution.md), and real ambient spectra of [Hermitian algebra elements](../../../../../hermitian-element-of-a-star-algebra.md) were used; the [C-star identity](../../../../../c-star-identity.md) was not assumed.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
