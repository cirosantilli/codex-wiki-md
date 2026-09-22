<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take compatible [function types](../../../../../function-type.md) `f :: b -> c`, `g :: b -> a -> b`, and `h :: c -> a -> c`. The necessary conditions obtained from the two [induction base cases](../../../../../induction-base-case.md) are **strictness of `f` and the fusion equation**

$$
f(\bot)=\bot,\qquad f(g\ x\ y)=h\ (f\ x)\ y\quad\text{for all }x,y.
$$

At `zs = []`, the desired equation is exactly the displayed fusion equation. At `zs = undefined`, both [left folds](../../../../../left-fold.md) diverge because their [list](../../../../../list-abstract-data-type.md) argument has no outer constructor; the equation therefore requires `f undefined = undefined`. This is the [strict function](../../../../../strict-function.md) condition. If only finite total spines were considered, the first condition would not be necessary.

These conditions also support the step. The [induction hypothesis](../../../../../induction-hypothesis.md) must hold for _every_ accumulator and element. For `z:zs`, instantiate that hypothesis at `g x y` and `z`:
```
f (foldl g (g x y) (z:zs))
 = f (foldl g (g (g x y) z) zs)
 = foldl h (h (f (g x y)) z) zs
 = foldl h (h (h (f x) y) z) zs
 = foldl h (h (f x) y) (z:zs).
```
The middle rewrite uses the fusion equation at `x,y`. For pure [computable functions](../../../../../computable-function.md), equality on infinite spines follows from finite approximations as in part (a).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
