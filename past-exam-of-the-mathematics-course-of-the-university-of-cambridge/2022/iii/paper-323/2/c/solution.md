<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $P_i=|y_i\rangle\langle y_i|$, the channel has Kraus form $Y(\rho)=\sum_iP_i\rho P_i$ and $\sum_iP_i^\dagger P_i=I$, so it is completely positive and trace preserving. It measures in the $y$ basis and prepares the observed basis state, hence is a [measure-and-prepare channel](../../../../../../measure-and-prepare-channel.md). If $p_i=\langle y_i|\rho|y_i\rangle$, then $Y(\rho)=\sum_ip_iP_i$ and

$$
\boxed{S(Y(\rho))=H(p)}.
$$

Moreover $\log Y(\rho)=\sum_i(\log p_i)P_i$ on its support, so

$$
\begin{aligned}
D(\rho\|Y(\rho))
&=\operatorname{Tr}(\rho\log\rho)-\sum_ip_i\log p_i\\
&=\boxed{S(Y(\rho))-S(\rho)}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
