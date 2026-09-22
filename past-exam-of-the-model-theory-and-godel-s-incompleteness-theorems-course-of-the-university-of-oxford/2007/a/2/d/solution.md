<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $d(n)$ be the [Gödel number](../../../../../godel-number.md) of the diagonal [first-order sentence](../../../../../first-order-sentence.md) obtained by substituting $\bar n$ into the one-free-variable [logical formula](../../../../../logical-formula.md) with code $n$, with an arbitrary default value on noncodes. By the assumptions and (c), this total [function](../../../../../function-split.md) has a strong defining [logical formula](../../../../../logical-formula.md) $D(x,y)$.

For the specified $F$, form the one-variable [logical formula](../../../../../logical-formula.md)

$$
H(x)=\exists y\,(D(x,y)\wedge F(y)).
$$

Let $h$ be the [Gödel number](../../../../../godel-number.md) of $H$ and put $C=H(\bar h)$. Then $d(h)=\ulcorner C\urcorner$. [Strong definability of a numerical function](../../../../../strong-definability-of-a-numerical-function.md) at this particular standard input gives

$$
S\vdash\forall y\,[D(\bar h,y)\leftrightarrow y=\overline{\ulcorner C\urcorner}].
$$

Substitution into the existential definition yields

$$
\boxed{S\vdash C\leftrightarrow F(\overline{\ulcorner C\urcorner}).}
$$

The permitted equivalence between the source's two substitution notations identifies this with its requested fixed point. [Bound variables](../../../../../bound-variable.md) are renamed when necessary before forming $H$, so the substitution is capture-free. This constructs one particular [first-order sentence](../../../../../first-order-sentence.md) from the code of the [logical formula](../../../../../logical-formula.md) which applies $F$ to its own diagonal output.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
