<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First suppose $(W,S)$ is a [Coxeter system](../../../../../../coxeter-system.md). The usual exchange condition implies that multiplication by a simple generator changes length by exactly one. Let $w=t_1\cdots t_n$ be reduced and suppose both $s_iw$ and $ws_j$ have length $n+1$. The length of $s_iws_j$ is therefore either $n+2$ or $n$. In the latter case, apply exchange to the reduced word $s_i t_1\cdots t_n$ followed by $s_j$. If exchange deleted one of the $t_k$, multiplying the resulting equality on the left by $s_i$ would express the length-$n+1$ element $ws_j$ using only $n-1$ generators. Hence exchange must delete the initial $s_i$, giving $s_iws_j=w$. This is exactly the folding condition.

Conversely, suppose the folding condition holds, and let $W_M$ be the abstract Coxeter group with generators $S$ and matrix $(m_{ij})$. The defining relations hold in $W$, so there is a surjective homomorphism

$$
\pi:W_M\longrightarrow W.
$$

It remains to prove injectivity. Take any word in the kernel. If its image word in $W$ is not reduced, choose its shortest nonreduced prefix $ut$, where $u$ is reduced and $t$ is its last generator. Part b gives $ut=v$, where $v$ is obtained by deleting one letter from $u$. Hence $u=vt$, and $u$ and $vt$ are two reduced expressions for the same element. By the assumed braid-equivalence theorem they are related by braid moves. Those moves are defining relations in $W_M$, after which the end of the prefix becomes $vtt$ and $t^2=1$ shortens the original word by two.

Repeating this process turns the kernel word, using only Coxeter relations, into a word that is reduced in $W$. Since its image is the identity, that reduced word is empty. The original word is therefore already the identity in $W_M$, so $\ker\pi=1$. Hence $W\cong W_M$ is the Coxeter group with generators $S$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
