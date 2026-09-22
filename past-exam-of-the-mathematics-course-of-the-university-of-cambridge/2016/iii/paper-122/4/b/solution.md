<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use right [comodules](../../../../../../comodule.md) and write their [coactions](../../../../../../coaction.md) as $u\mapsto\sum u_{(0)}\otimes u_{(1)}$. A [coquasitriangular structure](../../../../../../coquasitriangular-structure.md) gives the [braiding](../../../../../../braiding.md) on these [comodules](../../../../../../comodule.md)

$$
b_{M,N}(u\otimes v)=\sum v_{(0)}\otimes u_{(0)}\,\gamma(u_{(1)},v_{(1)}).
$$

In an arbitrary [symmetric monoidal category](../../../../../../symmetric-monoidal-category.md) this notation abbreviates a composite of the two coactions, the ambient symmetry, and $\gamma$; it does not assume that the objects have elements. The coquasitriangular axioms ensure that this composite is a comodule morphism, is invertible using the convolution inverse of $\gamma$, and satisfies the two hexagon laws. More explicitly, in scalar notation those laws come from

$$
\gamma(ab,c)=\sum\gamma(a,c_{(1)})\gamma(b,c_{(2)}),\qquad\gamma(a,bc)=\sum\gamma(a_{(1)},c)\gamma(a_{(2)},b),
$$

while the comodule-morphism condition is

$$
\sum\gamma(a_{(1)},b_{(1)})a_{(2)}b_{(2)}=\sum b_{(1)}a_{(1)}\gamma(a_{(2)},b_{(2)}).
$$

Unit normalizations give the unit constraints. These descriptions are identities of morphisms in the ambient symmetric category, with the displayed reordering carried by its symmetry.

Apply the preceding self-[braiding](../../../../../../braiding.md) result to the regular right [comodule](../../../../../../comodule.md) $(H,\Delta)$. Its [Yang–Baxter operator](../../../../../../yang-baxter-operator.md) is

$$
R(a\otimes b)=\sum b_{(1)}\otimes a_{(1)}\gamma(a_{(2)},b_{(2)}).
$$

Compose its braid equation with the three [counits](../../../../../../counit.md). Expanding $R_{23}R_{12}R_{23}$ and cancelling the leading counit factors gives

$$
\sum\gamma(a_{(1)},b_{(1)})\gamma(a_{(2)},c_{(1)})\gamma(b_{(2)},c_{(2)}).
$$

Expanding $R_{12}R_{23}R_{12}$ instead gives

$$
\sum\gamma(a_{(2)},b_{(2)})\gamma(b_{(1)},c_{(1)})\gamma(a_{(1)},c_{(2)}).
$$

They are equal by the [Yang–Baxter operator](../../../../../../yang-baxter-operator.md) equation. **This is the required scalar identity:**

$$
\boxed{\sum\gamma(a_{(1)},b_{(1)})\gamma(a_{(2)},c_{(1)})\gamma(b_{(2)},c_{(2)})=\sum\gamma(a_{(2)},b_{(2)})\gamma(b_{(1)},c_{(1)})\gamma(a_{(1)},c_{(2)}).}
$$

Indeed, after $\Delta^{\otimes3}$ the ordered factors are $a_{(1)},a_{(2)},b_{(1)},b_{(2)},c_{(1)},c_{(2)}$. The two ambient symmetries on the left produce the three pairings $(a_{(1)},b_{(1)})$, $(a_{(2)},c_{(1)})$, $(b_{(2)},c_{(2)})$. On the right, the central symmetry produces $a_{(1)},a_{(2)},b_{(2)},b_{(1)},c_{(1)},c_{(2)}$, yielding exactly the other three pairings. Hence the calculation identifies the actual morphisms requested, also when the category is not a category of vector spaces.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
