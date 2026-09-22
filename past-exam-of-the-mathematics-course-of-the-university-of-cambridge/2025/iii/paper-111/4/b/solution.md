<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove the assertion by induction on $n$. Write $w=av$, where $a=s_{i_1}$ and $v=s_{i_2}\cdots s_{i_n}$; both displayed words are reduced. The first clause of the [folding condition](../../../../../../folding-condition.md) and part a imply that $\ell(vs)$ is either $n-2$ or $n$.

If $\ell(vs)=n-2$, the induction hypothesis deletes one unique letter from the reduced word for $v$. Prefixing $a$ gives the required deletion from $w$. If another deletion were possible, induction rules out another internal position, while deletion of $a$ would give $ws=v$ and hence $vs=av$, contradicting the lengths $n-2$ and $n$.

If $\ell(vs)=n$, both $av$ and $vs$ increase the length of $v$. Since $\ell(avs)=\ell(ws)=n-1$, the other alternative in the folding condition must hold:

$$
v=avs.
$$

Thus $ws=avs=v$, which deletes the first letter. An additional internal deletion would give $v=a v'$ for a word $v'$ of length $n-2$; multiplying by $a$ would make the length-$n$ element $av=w$ equal to $v'$, impossible. The deletion position is therefore unique in every case.

## ↑ Ancestors (11)

1. [B](../b.md)
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
