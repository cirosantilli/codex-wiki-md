<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add the [abstract syntax tree](../../../../../abstract-syntax-tree.md) alternative `Fix Ident Expr`. Its [syntactic sugar](../../../../../syntactic-sugar.md) expansion and the semantic equations from part (a) give

$$
\begin{aligned}
\operatorname{eval}(\operatorname{Fix}\ x\ e)\,\rho
&=\operatorname{eval}(\operatorname{Let}\ (\operatorname{Rec}\ x\ e)\ (\operatorname{Variable}\ x))\,\rho\\
&=\operatorname{defn}(\operatorname{Rec}\ x\ e)\,\rho
\triangleright(\lambda\rho'.\,\operatorname{result}(\operatorname{lookupEnv}(\rho',x)))\\
&=\operatorname{result}(\rho^*)
\triangleright(\lambda\rho'.\,\operatorname{result}(\operatorname{lookupEnv}(\rho',x)))\\
&=\operatorname{result}(v),
\end{aligned}
$$

where $\rho^*=\operatorname{extend}(\rho,[(x,v)])$ and $v=\operatorname{close}(e,\rho^*)$. The final step uses left identity from the [monad laws](../../../../../monad-laws.md) and the lookup rule for the newly bound identifier.

Thus a direct evaluator equation is:

```
eval (Fix x e@(Lambda xs body)) rho = result v
  where
    rho' = extend rho [(x,v)]
    v = close e rho'
```

Equivalently, spelling out [programming closure](../../../../../closure-computer-programming.md) construction,

$$
\boxed{\operatorname{eval}(\operatorname{Fix}\ x\ (\operatorname{Lambda}\ xs\ b))\,\rho
=\operatorname{result}(v),\quad
v=\operatorname{Function}\bigl(\lambda args.\,
\operatorname{eval}(b)(\operatorname{extend}(\rho^*,\operatorname{zip}(xs,args)))\bigr).}
$$

The result is a [recursive closure](../../../../../recursive-closure.md), not the result of calling its body. Its self-binding is visible inside that body but does not extend the caller's surrounding [semantic environment](../../../../../semantic-environment.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
