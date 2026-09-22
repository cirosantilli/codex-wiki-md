<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The local criterion states that an $R$-module $M$ is flat if and only if $M_{\mathfrak p}$ is flat over $R_{\mathfrak p}$ for every prime ideal $\mathfrak p$. It is enough equivalently to test maximal ideals.

If $M$ is flat, localization of an exact sequence and the natural isomorphism

$$
(M\otimes_RN)_{\mathfrak p}
\cong M_{\mathfrak p}\otimes_{R_{\mathfrak p}}N_{\mathfrak p}
$$

show immediately that every $M_{\mathfrak p}$ is flat.

Conversely, let $N'\to N$ be injective and let $K$ be the kernel of

$$
M\otimes_RN'\longrightarrow M\otimes_RN.
$$

After localization at any prime $\mathfrak p$, flatness of $M_{\mathfrak p}$ gives $K_{\mathfrak p}=0$. A module whose localization at every maximal ideal is zero must itself be zero: if $0\ne x\in K$, its annihilator is contained in a maximal ideal $\mathfrak m$, and then $x/1\ne0$ in $K_{\mathfrak m}$. Hence $K=0$, tensoring by $M$ preserves every injection, and $M$ is flat. This proves that [flatness is local](../../../../../../flatness-is-local.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
