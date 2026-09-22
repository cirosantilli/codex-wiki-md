<h1 id="12i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the intercepted ciphertext, known plaintext, and desired plaintext without spaces:

$$
C=\text{LRPFOJQLCUD},\qquad
P=\text{FLYXATXONCE},\qquad
P'=\text{REMAINXHERE}.
$$

Because the pad is additive, Eve applies the [malleability of an additive one-time pad](../../../../../../malleability-of-an-additive-one-time-pad.md) and sends

$$
C'=C-P+P'\pmod{26}.
$$

Letter-by-letter, using $A=1,\ldots,Z=26$, this gives

$$
\begin{array}{c|ccccccccccc}
C&L&R&P&F&O&J&Q&L&C&U&D\\
P&F&L&Y&X&A&T&X&O&N&C&E\\
P'&R&E&M&A&I&N&X&H&E&R&E\\ \hline
C'&X&K&D&I&W&D&Q&E&T&J&D
\end{array}
$$

Thus Eve should deliver

$$
\boxed{\text{XKDIWDQETJD}.}
$$

Indeed, if $C=P+K$, then $C'=C-P+P'=P'+K$, so Ollie decrypts the desired message.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12I](../../12i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
