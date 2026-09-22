<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [diagonal lemma](../../../../../../diagonal-lemma.md) says that for every one-variable formula $\theta(x)$ there is a sentence $\gamma$ such that

$$
T\vdash\gamma\leftrightarrow\theta(\ulcorner\gamma\urcorner).
$$

Let $d(n)$ be the computable function taking the code of a one-variable formula $\alpha(x)$ to the code of $\alpha(\bar n)$. By the assumed representation theorem, choose a Sigma-1 formula $D(x,y)$ representing $d$. Given $\theta$, put

$$
\beta(x)=\exists y\bigl(D(x,y)\wedge\theta(y)\bigr)
$$

and let $b=\ulcorner\beta\urcorner$. Taking $\gamma=\beta(\bar b)$, representability proves in $T$ that the unique relevant $y$ is $d(b)=\ulcorner\gamma\urcorner$, yielding the required equivalence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
