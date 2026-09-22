<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The kernel of the restriction map

$$
\Gamma(X,\mathcal F)\longrightarrow\Gamma(X\setminus Z,\mathcal F)
$$

consists exactly of sections whose germs vanish outside $Z$, namely $\Gamma_Z(X,\mathcal F)$. This proves exactness. If $\mathcal F$ is a [flasque sheaf](../../../../../../flasque-sheaf.md), the restriction map is surjective by definition.

Now let $0\to\mathcal F_1\to\mathcal F_2\to\mathcal F_3\to0$ be exact. The [global section functor](../../../../../../global-section-functor.md) is left exact, so a section of $\Gamma_Z(X,\mathcal F_2)$ mapping to zero lifts uniquely to a global section of $\mathcal F_1$. Its germs outside $Z$ vanish because $\mathcal F_1\to\mathcal F_2$ is injective at each [stalk of a sheaf](../../../../../../stalk-of-a-sheaf.md). It therefore lies in $\Gamma_Z(X,\mathcal F_1)$, proving exactness of the supported-section sequence.

Suppose in addition that $\mathcal F_1$ is flasque and take $s_3\in\Gamma_Z(X,\mathcal F_3)$. Surjectivity on global sections gives a lift $s_2\in\Gamma(X,\mathcal F_2)$. On $X\setminus Z$, its restriction comes from some $t_1\in\Gamma(X\setminus Z,\mathcal F_1)$ by left exactness. Extend $t_1$ to $\widetilde t_1\in\Gamma(X,\mathcal F_1)$ using flasqueness. Then $s_2-\widetilde t_1$ maps to $s_3$ and vanishes outside $Z$, proving surjectivity on the right.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
