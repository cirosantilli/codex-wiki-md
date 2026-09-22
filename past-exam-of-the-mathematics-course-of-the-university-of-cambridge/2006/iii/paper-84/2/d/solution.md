<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [four-input parity network](../../../../../../four-input-parity-network.md). Let $S=z_1+z_2+z_3+z_4$. Four [hidden units](../../../../../../hidden-unit.md) each receive all inputs with weight one and have thresholds $1/2,3/2,5/2,7/2$. Thus

$$
h_m=H(S-m+\tfrac12),\qquad m=1,2,3,4,
$$

where $H(a)=1$ for $a\geq0$ and zero otherwise. The output receives weights $(1,-1,1,-1)$ and has threshold $1/2$:

$$
\boxed{y=H(h_1-h_2+h_3-h_4-\tfrac12)}.
$$

The computation depends only on input count, so the following table checks all sixteen patterns at once:

$$
\begin{array}{c|c|c|c}
S&(h_1,h_2,h_3,h_4)&h_1-h_2+h_3-h_4&y\\\hline
0&(0,0,0,0)&0&0\\
1&(1,0,0,0)&1&1\\
2&(1,1,0,0)&0&0\\
3&(1,1,1,0)&1&1\\
4&(1,1,1,1)&0&0
\end{array}
$$

**The output is one exactly for an odd input count.** The hidden features detect nested count thresholds, whose alternating sum extracts odd parity.

This representation does not make learning automatically easy. Hard [binary threshold units](../../../../../../binary-threshold-unit.md) have no usable ordinary derivative; [backpropagation](../../../../../../backpropagation.md) normally uses smooth approximations. With uniformly sampled parity patterns, each individual input has zero correlation with the target, so simple first-order features provide no direct cue to the required interaction. The desired output also flips between neighboring count classes. A smooth network has sufficient capacity, but its training can be sensitive to initialization, saturation and local optimization; representability and trainability are different issues.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
