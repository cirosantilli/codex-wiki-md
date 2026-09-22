<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Downward Lowenheim-Skolem theorem](../../../../../downward-lowenheim-skolem-theorem.md) says that for an $L$-structure $M$ and a [subset](../../../../../subset.md) $S\subseteq M$, there is an [elementary substructure](../../../../../elementary-substructure.md) $N\preccurlyeq M$ containing $S$ with

$$
\boxed{|N|\le\max(|S|,|L|,\aleph_0).}
$$

If an infinite cardinal $\kappa$ satisfies $\max(|L|,\aleph_0)\le\kappa\le|M|$, one can in particular obtain size exactly $\kappa$ by starting with a [subset](../../../../../subset.md) of that size.

Choose a default element $a_0\in M$. For every [logical formula](../../../../../logical-formula.md) $\exists x\phi(x,\vec y)$ choose a [Skolem function](../../../../../skolem-function.md) $F_\phi$ which returns a witness in $M$ when one exists, and returns $a_0$ otherwise. Begin with $S$, the interpretations of the [first-order language](../../../../../first-order-language.md)'s constants, and $a_0$. Successively adjoin the values of all the original [functions](../../../../../function-split.md) and these [Skolem functions](../../../../../skolem-function.md) on finite [tuples](../../../../../finite-tuple.md) already chosen. Let $N$ be the [union](../../../../../set-union.md) of the resulting [countable](../../../../../countable-set.md) sequence of closure stages.

There are at most $\max(|L|,\aleph_0)$ [logical formulas](../../../../../logical-formula.md), and each [function](../../../../../function-split.md) has finite arity. With $\kappa=\max(|S|,|L|,\aleph_0)$, each closure stage has size at most $\kappa$, and so does their [countable](../../../../../countable-set.md) [union](../../../../../set-union.md). Closure under the original [functions](../../../../../function-split.md) makes $N$ an $L$-substructure. Whenever $M\models\exists x\phi(x,\vec a)$ for parameters in $N$, its chosen Skolem witness belongs to $N$, since the finitely many parameters lie in some common stage. The Tarski–Vaught test therefore gives $N\preccurlyeq M$.

For the exact-cardinality version, choose an initial [set](../../../../../set-split.md) of $\kappa$ elements, enlarged to contain any prescribed [subset](../../../../../subset.md) of size at most $\kappa$. The construction gives an upper bound $\kappa$ while containment gives the matching lower bound.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
