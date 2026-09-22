<h1 id="2/11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Suppose $K$ is a [compact operator](../../../../../../compact-operator-split.md) and $f_n\rightharpoonup f$. The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) makes $(f_n)$ bounded. If $Kf_n$ did not converge in norm to $Kf$, some subsequence would stay a fixed positive distance away. Compactness provides a further norm-convergent subsequence, say to $g$. On the other hand, for every $h$, $\langle Kf_n,h\rangle=\langle f_n,K^*h\rangle\to\langle Kf,h\rangle$, so its norm limit must be $Kf$, a contradiction.

Conversely, if $K$ sends every weakly convergent sequence to a norm-convergent sequence, take any sequence in the closed [unit ball](../../../../../../unit-ball.md). Weak compactness of that ball supplies a weakly convergent subsequence, whose images converge in norm by hypothesis. Thus every sequence in the image has a convergent subsequence in $H$. Its closure is also sequentially compact: approximate its $n$th member by an image point within $1/n$. Since $H$ is a [metric space](../../../../../../metric-space.md), that closure is compact. We conclude

$$
\boxed{K\text{ compact}\iff f_n\rightharpoonup f\Longrightarrow\|Kf_n-Kf\|\to0.}
$$

This is the principle that [compact operators send weak convergence to norm convergence](../../../../../../compact-operators-send-weak-convergence-to-norm-convergence.md).

## ↑ Ancestors (11)

1. [11](../11.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
