<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

One choice of the [Hamming code of length seven](../../../../../hamming-code-of-length-seven.md) is the [linear map](../../../../../linear-map.md)

$$
h(a,b,c,d)=(a+b+d,\ a+c+d,\ a,\ b+c+d,\ b,\ c,\ d)
$$

over $\mathbb F_2$. Its image is the [kernel](../../../../../kernel-of-a-linear-map.md) of the [parity-check matrix](../../../../../parity-check-matrix.md)

$$
H=\begin{pmatrix}1&0&1&0&1&0&1\\0&1&1&0&0&1&1\\0&0&0&1&1&1&1\end{pmatrix}.
$$

Indeed $Hh(a,b,c,d)^T=0$, the encoder is [injective](../../../../../injective-function.md) because positions $3,5,6,7$ recover its inputs, and $H$ has [rank](../../../../../rank-one-quadratic-form.md) three. Its columns are nonzero and pairwise distinct. Hence no nonzero [codeword](../../../../../codeword.md) has [Hamming weight](../../../../../hamming-weight.md) one or two. The word $h(1,0,0,0)=(1,1,1,0,0,0,0)$ has weight three, proving that the [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) is **three**.

If $r=h(a,b,c,d)+e_j$ is received with one erroneous bit, its [syndrome](../../../../../syndrome.md) $Hr^T$ is column $j$ of $H$. These seven columns are distinct, so the [syndrome](../../../../../syndrome.md) identifies the bit to flip. A zero [syndrome](../../../../../syndrome.md) indicates no error under the assumption of at most one error.

For the [extended Hamming code](../../../../../extended-hamming-code.md), append $\sum_{j=1}^7h_j=a+b+c$. Every extended [codeword](../../../../../codeword.md) has [even](../../../../../even-function.md) weight. Since every original nonzero word has weight at least three, its extended weight is at least four; the weight-three example attains four. Thus

$$
\boxed{d_{\min}=4.}
$$

The [minimum-distance error-detection and correction guarantee](../../../../../minimum-distance-error-detection-and-correction-guarantee.md) gives **detection of up to three errors and correction of one error**. Detection here means rejecting a word outside the code, rather than simultaneously identifying and correcting every detected pattern; the usual combined decoder corrects single errors and flags double errors.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
