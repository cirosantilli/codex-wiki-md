<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a covector $p\in T_x^*X$, define the [cotangent lift of a diffeomorphism](../../../../../../cotangent-lift-of-a-diffeomorphism.md) by

$$
\boxed{f_\#(x,p)=\bigl(f(x),p\circ(df_x)^{-1}\bigr).}
$$

The inverse derivative here maps $T_{f(x)}X$ to $T_xX$. This is a smooth [diffeomorphism](../../../../../../diffeomorphism.md), its inverse is $(f^{-1})_\#$, and it satisfies $\pi\circ f_\#=f\circ\pi$.

For $v\in T_{(x,p)}T^*X$, the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) and the defining formula for the [Liouville one-form](../../../../../../canonical-one-form-on-a-cotangent-bundle.md) give

$$
\begin{aligned}
(f_\#^*\alpha)_{(x,p)}(v)
&=(p\circ(df_x)^{-1})\bigl(d\pi_{f_\#(x,p)}df_\#(v)\bigr)\\
&=(p\circ(df_x)^{-1})(df_xd\pi_{(x,p)}v)\\
&=p(d\pi_{(x,p)}v)=\alpha_{(x,p)}(v).
\end{aligned}
$$

Hence **$f_\#^*\alpha=\alpha$**, and applying the [exterior derivative](../../../../../../exterior-derivative.md) also proves $f_\#^*\omega=\omega$. The [cotangent lift of a diffeomorphism](../../../../../../cotangent-lift-of-a-diffeomorphism.md) thus preserves both canonical forms, with no extra choice of metric or connection.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
