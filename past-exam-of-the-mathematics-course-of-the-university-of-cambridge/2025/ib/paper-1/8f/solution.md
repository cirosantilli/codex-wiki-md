<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

For a [linear map](../../../../../linear-map.md) $T:V\to W$ with $V$ finite-dimensional,

$$
\dim V=\operatorname{rk}T+\dim\ker T.
$$

Now

$$
\operatorname{rk}(\alpha\beta)=\dim\operatorname{im}\beta-dim(\ker\alpha\cap\operatorname{im}\beta)
\ge\operatorname{rk}\beta-\dim\ker\alpha,
$$

which is the required inequality after rank-nullity for $\alpha$.

If $X$ and $Y$ represent the same map, then $Y=C^{-1}XB$, where $B$ changes new domain coordinates to old ones and $C$ does the same in the codomain.

Invertible block row and column operations reduce

$$
\begin{pmatrix}P&Q\\R&S\end{pmatrix}
$$

to $\operatorname{diag}(P,S-RP^{-1}Q)$, proving the rank formula. Apply it to $\begin{pmatrix}I_n&Q\\R&I_m\end{pmatrix}$ first with the upper-left block and then with the lower-right block. Equating the results gives

$$
\boxed{\operatorname{rk}(I_n-QR)=\operatorname{rk}(I_m-RQ)+n-m.}
$$

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
