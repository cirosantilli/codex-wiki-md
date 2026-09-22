<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the [monoidal category](../../../../../../monoidal-category.md) of [modules](../../../../../../module-mathematics.md) over the [commutative ring](../../../../../../commutative-ring.md) $k$, consider the [monad](../../../../../../monad.md) $T=H\otimes_k-$ coming from the unit and multiplication of the [bialgebra](../../../../../../bialgebra.md) $H$. Its [opmonoidal functor](../../../../../../opmonoidal-functor.md) structure has comparison maps

$$
T_2\bigl(h\otimes(x\otimes y)\bigr)=\sum(h_{(1)}\otimes x)\otimes(h_{(2)}\otimes y),\qquad T_0=\varepsilon:H\otimes_k k\cong H\to k.
$$

Here and below [Sweedler notation](../../../../../../sweedler-notation.md) abbreviates the [comultiplication](../../../../../../comultiplication.md) $\Delta h=\sum h_{(1)}\otimes h_{(2)}$. The opmonoidal associativity and unit axioms are the coassociativity and counit laws of the [coalgebra](../../../../../../coalgebra.md). The [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md) are [opmonoidal natural transformations](../../../../../../opmonoidal-natural-transformation.md) because the [bialgebra](../../../../../../bialgebra.md) axioms say

$$
\Delta(hg)=\sum h_{(1)}g_{(1)}\otimes h_{(2)}g_{(2)},\qquad\Delta(1)=1\otimes1,\qquad\varepsilon(hg)=\varepsilon(h)\varepsilon(g),\quad\varepsilon(1)=1.
$$

The [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) of this [opmonoidal monad](../../../../../../opmonoidal-monad.md) is the category of left $H$-[modules](../../../../../../module-mathematics.md): a monad-algebra map $H\otimes_kM\to M$ is exactly a unital associative action.

Applying the preceding construction gives the [diagonal bialgebra action](../../../../../../diagonal-bialgebra-action.md) and the unit action

$$
\boxed{h\cdot(u\otimes v)=\sum(h_{(1)}\cdot u)\otimes(h_{(2)}\cdot v),\qquad h\cdot a=\varepsilon(h)a\quad(a\in k).}
$$

The usual [associators](../../../../../../associator.md) and [unitors](../../../../../../unitor.md) for the [tensor product of modules](../../../../../../tensor-product-of-modules.md) are $H$-linear, and the underlying tensor product is exactly $\otimes_k$. **The forgetful functor into $k$-modules is strict monoidal.** The base need not be a [field](../../../../../../field.md); the [modules](../../../../../../module-mathematics.md) need be neither [flat modules](../../../../../../flat-module.md) nor [finitely generated modules](../../../../../../finitely-generated-module.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
