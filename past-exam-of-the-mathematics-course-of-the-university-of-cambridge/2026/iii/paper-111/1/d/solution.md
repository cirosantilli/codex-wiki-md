<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $N(w)$ for the [inversion set of a Weyl-group element](../../../../../../inversion-set-of-a-weyl-group-element.md). Part b shows that $s_\alpha$ permutes $\Pi\setminus\{\alpha\}$. It follows that right multiplication by $s_\alpha$ changes the size of the inversion set by

$$
|N(ws_\alpha)|=
\begin{cases}
|N(w)|+1,&w(\alpha)\in\Pi,\\
|N(w)|-1,&w(\alpha)\in-\Pi.
\end{cases}
$$

Indeed, all roots other than $\alpha$ are merely relabelled, while $ws_\alpha(\alpha)=-w(\alpha)$. Part c gives exactly the same recursion for the [Coxeter length](../../../../../../coxeter-length.md). Both quantities vanish at the identity, so induction along any word in the simple reflections gives

$$
\boxed{\ell(w)=|N(w)|
=\left|\{\beta\in\Pi:w(\beta)\in-\Pi\}\right|.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
