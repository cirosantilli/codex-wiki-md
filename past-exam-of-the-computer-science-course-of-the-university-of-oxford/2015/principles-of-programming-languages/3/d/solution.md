<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Add `Fixes [Ident] [Expr]` to the [abstract syntax tree](../../../../../abstract-syntax-tree.md). For the stipulated nonempty, equally long lists of distinct names and [lambda abstractions](../../../../../lambda-abstraction.md), define all [programming closures](../../../../../closure-computer-programming.md) against one common extended [semantic environment](../../../../../semantic-environment.md):

```
eval (Fixes xs es) rho = result (head vs)
  where
    rho' = extend rho (zip xs vs)
    vs = map (\e -> close e rho') es
```

Expanding the auxiliary [function](../../../../../function-split.md), if $e_i=\operatorname{Lambda}\ ys_i\ b_i$,

$$
\boxed{\begin{aligned}
\rho^*&=\operatorname{extend}(\rho,[(x_1,v_1),\ldots,(x_n,v_n)]),\\
v_i&=\operatorname{Function}\bigl(\lambda args.\,
\operatorname{eval}(b_i)(\operatorname{extend}(\rho^*,\operatorname{zip}(ys_i,args)))\bigr),\\
\operatorname{eval}(\operatorname{Fixes}\ [x_1,\ldots,x_n]\ [e_1,\ldots,e_n])\,\rho
&=\operatorname{result}(v_1).
\end{aligned}}
$$

Every body can therefore call every member of the family, including itself. Constructing the family performs no body computations in the arbitrary [computational monad](../../../../../computational-monad.md). As in part (c), host [lazy evaluation](../../../../../lazy-evaluation.md) ties the recursive [semantic environment](../../../../../semantic-environment.md); a monadic fixed-point operator is unnecessary.

For example, with two bodies implementing evenness and oddness, respectively, each [programming closure](../../../../../closure-computer-programming.md) sees both names in $\rho^*$. Returning the first [programming closure](../../../../../closure-computer-programming.md) still retains access to the second. Building each [programming closure](../../../../../closure-computer-programming.md) in an independently extended old [semantic environment](../../../../../semantic-environment.md) would lose this [mutual recursion](../../../../../mutual-recursion.md). For $n=1$, the definition agrees with `Fix`.

## ↑ Ancestors (11)

1. [D](../d.md)
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
