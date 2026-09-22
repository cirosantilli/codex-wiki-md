<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A realized message $x$ has [self-information](../../../../information-content.md) $I(x)=-\log_2p_x$. The average information per source message is its [Shannon entropy](../../../../information-entropy-split.md),

$$
\boxed{H(M)=-p_A\log_2p_A-p_B\log_2p_B-p_C\log_2p_C.}
$$

The average reaches **$\log_2 3\simeq1.58496$ bits per message** at $p_A=p_B=p_C=1/3$. Individual rare realizations can have larger self-information; this bound concerns the average.

The given strings form a [prefix code](../../../../prefix-code.md) with lengths $\ell_A=1$ and $\ell_B=\ell_C=2$. To attain the entropy bound without redundancy, the resulting long bit stream must carry one bit of information per bit: unbiased bits with no predictable dependence. For an independent source, the [dyadic source matched to a complete prefix code](../../../../dyadic-source-matched-to-a-complete-prefix-code.md) has

$$
\boxed{p_A=2^{-1}=\frac12,\qquad p_B=p_C=2^{-2}=\frac14.}
$$

These probabilities make the encoded stream equivalent to parsing independent fair bits using the code tree. Its [expected codeword length](../../../../expected-codeword-length.md) and source entropy agree:

$$
\boxed{\overline\ell=H(M)=\frac12\cdot1+\frac14\cdot2+\frac14\cdot2=\frac32\ \text{bits per message}.}
$$

Here “optimal” means attaining the Shannon bound. If it means only an [optimal prefix code](../../../../optimal-prefix-code.md) among symbol-by-symbol binary prefix codes, the probabilities are not unique: for three positive-probability symbols, this tree is optimal whenever $p_A$ is a largest probability. [Huffman coding](../../../../huffman-coding.md) need not attain entropy exactly for nondyadic probabilities.

Concatenating the specified source-message encodings gives

$$
AABCACBA\ \longmapsto\ 0\,|\,0\,|\,10\,|\,11\,|\,0\,|\,11\,|\,10\,|\,0
=001011011100.
$$

Pack consecutive bits in pairs, rather than allocating a fresh Bell pair to each variable-length source word:

$$
00\,|\,10\,|\,11\,|\,01\,|\,11\,|\,00.
$$

Under the mapping in part 1, transmit

$$
\boxed{\Phi^+,\ \Phi^-,\ \Psi^-,\ \Psi^+,\ \Psi^-,\ \Phi^+.}
$$

The block uses six message-bearing qubit transmissions and six preshared [Bell pairs](../../../../bell-pair.md). Source-message boundaries are recovered by parsing the decoded prefix bit stream.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [7](../../7-split.md)
3. [2006](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
