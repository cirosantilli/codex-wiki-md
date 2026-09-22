<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Part (a)(i), applied to $w=u$ and $g=\overline u x$, guarantees an accepted output of length at most $m+N$. Its [padded convolution of words](../../../../../../padded-convolution-of-words.md) has at most $m+N$ columns. Thus the [dynamic programming](../../../../../../dynamic-programming.md) search in part (b) reaches an accepting layer by this bound.

Each layer has at most twice the fixed number of states of $M_x$, and each record has at most $|A|+1$ outgoing choices. These are constants for the fixed [automatic structure for a group](../../../../../../automatic-structure-for-a-group.md). Storing a pointer and a symbol takes constant time; copying whole partial output strings at every step would unnecessarily spoil this bound. Reconstruction also takes at most $m+N$ steps. Therefore **automatic multiplication has linear time and bounded length increase**:

$$
\boxed{|v|\leq |u|+N,\qquad T(u,x)=O(|u|+1).}
$$

For nonempty inputs this is the requested $O(|u|)$ [time complexity](../../../../../../time-complexity.md). The additive $1$ merely includes the constant work on the [empty word](../../../../../../empty-word.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
