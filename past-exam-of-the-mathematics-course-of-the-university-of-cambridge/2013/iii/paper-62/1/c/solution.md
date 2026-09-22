<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $C=\operatorname{conv}\{a,b\}$. Maximizing a linear functional over this line segment occurs at an endpoint, so

$$
f(x)=\sigma_C(x)=\sup_{p\in C}\langle p,x\rangle.
$$

This identifies $f$ as a [support function](../../../../../../support-function.md). Its [convex conjugate](../../../../../../convex-conjugate.md) is the [indicator functional](../../../../../../indicator-functional-of-a-constraint-set.md) $\delta_C$: if $p\in C$, then $\langle p,x\rangle-\sigma_C(x)\leq0$ for every $x$, with equality at zero; if $p\notin C$, strict separation and positive scaling of the separating vector make the supremum infinite.

For a [convex function](../../../../../../convex-function.md), equality in the [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md) characterizes its [subdifferential](../../../../../../subdifferential.md). Hence

$$
p\in\partial f(x)
\iff p\in C\ \text{and}\ \langle p,x\rangle=\sigma_C(x).
$$

This is [support-function subgradients as exposed faces](../../../../../../support-function-subgradients-as-exposed-faces.md). In particular a maximizing $p$ really is a [subgradient](../../../../../../subgradient.md), since $\sigma_C(z)\geq\langle p,z\rangle=f(x)+\langle p,z-x\rangle$ for every $z$.

Writing $p=ta+(1-t)b$, with $0\leq t\leq1$, now gives

$$
\boxed{\partial f(x)=
\begin{cases}
\{a\},&a^Tx>b^Tx,\\
\{b\},&b^Tx>a^Tx,\\
\operatorname{conv}\{a,b\},&a^Tx=b^Tx.
\end{cases}}
$$

If $a=b$, the last line is the singleton $\{a\}$, so the formula includes that case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
