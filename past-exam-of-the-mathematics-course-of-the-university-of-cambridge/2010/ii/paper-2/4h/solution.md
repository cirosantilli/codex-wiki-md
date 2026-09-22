<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

Take the [parity-check matrix](../../../../../parity-check-matrix.md)

$$
H=\begin{pmatrix}0&0&0&1&1&1&1\\0&1&1&0&0&1&1\\1&0&1&0&1&0&1\end{pmatrix}
$$

over $\mathbb F_2$. Its columns are all the nonzero vectors of $\mathbb F_2^3$. The [Hamming code](../../../../../hamming-code.md) is $C=\ker H$. Since $H$ has rank three, $C$ is a binary [linear code](../../../../../linear-code.md) of length seven and dimension four. No nonzero [codeword](../../../../../codeword.md) has weight one or two, since no column is zero and no two columns coincide. Columns $u,v,u+v$ give a [codeword](../../../../../codeword.md) of weight three, so **$C$ has parameters $[7,4,3]$.**

For a received vector $w=c+e$, its [syndrome](../../../../../syndrome.md) is $Hw=He$. A single error in position $j$ gives exactly column $j$ of $H$, so the [syndrome](../../../../../syndrome.md) identifies that position uniquely; zero [syndrome](../../../../../syndrome.md) means no error under the one-error assumption. The radius-one [Hamming balls](../../../../../hamming-ball.md) around the $16$ [codewords](../../../../../codeword.md) are disjoint and have total size $16(1+7)=128=2^7$, so this is also a [perfect code](../../../../../perfect-code.md).

There are $\binom72/3=7$ weight-three [codewords](../../../../../codeword.md): every pair of columns determines the third, and each triple is counted three times. The all-ones vector is a [codeword](../../../../../codeword.md) because the column sum is zero, so complementation gives seven weight-four [codewords](../../../../../codeword.md). Together with zero and the all-ones vector these account for all sixteen. The [weight enumerator](../../../../../weight-enumerator.md) is therefore

$$
\boxed{W_C(z)=1+7z^3+7z^4+z^7}.
$$

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
