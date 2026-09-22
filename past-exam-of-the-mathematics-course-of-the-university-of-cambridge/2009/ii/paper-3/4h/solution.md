<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

Use the binary [Hamming code](../../../../../hamming-code.md) $C=\ker H\subset\mathbb F_2^{15}$, where the $j$th column $h_j$ of the $4\times15$ [parity-check matrix](../../../../../parity-check-matrix.md) $H$ is the four-digit binary expansion of $j$, for $1\le j\le15$. Thus the columns are precisely the nonzero vectors of $\mathbb F_2^4$. They include the four coordinate vectors, so $\operatorname{rank}H=4$ and $\dim C=15-4=11$. Its [code rate](../../../../../code-rate.md) is therefore $\boxed{11/15}$.

For a received word $y$, compute its [syndrome](../../../../../syndrome.md) $s=Hy$. If $s=0$, report no error. Otherwise identify the unique column $h_j=s$ and flip bit $j$. Indeed, if $y=c+e_j$ with $c\in C$, then $Hy=Hc+He_j=h_j$, so this procedure recovers $c$ exactly. No column is zero and no two columns coincide; hence no nonzero [codeword](../../../../../codeword.md) has [Hamming weight](../../../../../hamming-weight.md) one or two. Some three columns sum to zero, for example those indexed by $1,2,3$, so the [minimum distance](../../../../../minimum-distance-of-a-code.md) is exactly three. Thus **every single-bit error is corrected**. The assertion requires at most one error; arbitrary multiple errors need not be detected by this procedure.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
