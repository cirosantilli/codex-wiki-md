<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use three states of a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md): disease-free $1$, pre-clinical $2$, and clinical $3$. The [transition intensities](../../../../../../transition-intensity.md) are $\lambda=q_{12}>0$ for onset and $\nu=q_{23}>0$ for progression. Clinical disease is an [absorbing state](../../../../../../absorbing-state.md). The mandatory pre-clinical phase excludes a direct $1\to3$ jump, and this untreated progression model has no reverse transitions.

<a id="2/a/image-irreversible-cancer-progression-from-disease-free-to-pre-clinical-to-clinical-states"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207-cancer-states.png)

**[Figure 1](#2/a/image-irreversible-cancer-progression-from-disease-free-to-pre-clinical-to-clinical-states). Irreversible cancer progression from disease-free to pre-clinical to clinical states**.

With row-vector probabilities and state order $(1,2,3)$, **the generator matrix** is

$$
\boxed{Q=\begin{pmatrix}-\lambda&\lambda&0\\0&-\nu&\nu\\0&0&0\end{pmatrix}.}
$$

Its rows sum to zero, so only the two off-diagonal [transition intensities](../../../../../../transition-intensity.md) are unknown. This is a [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) with sequential irreversible progression.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
