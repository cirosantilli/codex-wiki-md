<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

Use [simplicial homology](../../../../../simplicial-homology.md) with a fixed coefficient group or ring. The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) is

$$
\cdots\longrightarrow H_{i+1}(X)\xrightarrow{\delta}H_i(A\cap B)
\xrightarrow{\alpha}H_i(A)\oplus H_i(B)
\xrightarrow{\beta}H_i(X)\xrightarrow{\delta}H_{i-1}(A\cap B)\longrightarrow\cdots.
$$

The inclusion maps define $\alpha([z])=([z],-[z])$ and $\beta([a],[b])=[a+b]$. To define $\delta$, split a [simplicial cycle](../../../../../simplicial-cycle.md) $c\in C_{i+1}(X)$ as $c=a+b$ with $a$ a chain in $A$ and $b$ in $B$. Since $\partial a=-\partial b$, this boundary lies in $C_i(A\cap B)$, and $\delta[c]=[\partial a]$. At degree zero the unreduced sequence ends with $H_0(A)\oplus H_0(B)\to H_0(X)\to0$.

If $[z]=\delta[c]$, its representative is a boundary in $A$ and the negative of a boundary in $B$, so $\alpha[z]=0$. Thus $\operatorname{im}\delta\subseteq\ker\alpha$.

Conversely if $\alpha[z]=0$, choose $a\in C_{i+1}(A)$ and $b\in C_{i+1}(B)$ with $\partial a=z=\partial b$. The chain $c=a-b$ is a [simplicial cycle](../../../../../simplicial-cycle.md) in $X$. Its splitting into the $A$ chain $a$ and $B$ chain $-b$ gives $\delta[c]=[z]$. Hence **$\operatorname{im}\delta=\ker\alpha$**, the requested exactness at $H_i(A\cap B)$.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
