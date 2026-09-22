<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the outermost boxed subformulas of $X(p)$ containing the distinguished letter. Because $X$ is modalized in $p$, every occurrence of $p$ lies inside one of these boxes. The supplied decomposition therefore has the form

$$
X(p)=H(\Box C_1(p),\ldots,\Box C_m(p)),
$$

where $H$ has no occurrence of $p$. Other letters and subformulas not involving $p$ may be retained as parameters in $H$ and the $C_i$.

Introduce temporary letters $q_1,\ldots,q_m$ and solve the boxed system

$$
q_i\leftrightarrow\Box C_i(H(q_1,\ldots,q_m))
$$

by part (b), obtaining $Q_i$ without the temporary letters or $p$. Put $F=H(Q_1,\ldots,Q_m)$. Each solved equation gives $GL\vdash Q_i\leftrightarrow\Box C_i(F)$. The supplied replacement-of-equivalents principle then gives

$$
\boxed{GL\vdash F\leftrightarrow H(\Box C_1(F),\ldots,\Box C_m(F))=X(F).}
$$

Only letters already present in $X$, apart from the removed $p$, occur in the constructed $F$. If $p$ is absent from $X$ to begin with, take $F=X$. This is the [modalized fixed-point theorem for GL](../../../../../modalized-fixed-point-theorem-for-gl.md), proved by finite elimination rather than a semantic completeness argument.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
