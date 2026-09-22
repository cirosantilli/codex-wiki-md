<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [agglomerative hierarchical clustering](../../../../../../agglomerative-hierarchical-clustering.md), start with eight singleton groups. [Single-linkage clustering](../../../../../../single-linkage-clustering.md) uses the smallest distance between cross-pairs; [complete-linkage clustering](../../../../../../complete-linkage-clustering.md) uses the largest. Updating these cluster distances after each merge, one valid order of the tied merges gives

$$
\begin{array}{c|cc|cc}
\text{step}&\text{single cluster}&\text{height}&\text{complete cluster}&\text{height}\\\hline
1&BD&0.4&BD&0.4\\
2&AC&0.6&AC&0.6\\
3&EG&0.6&EG&0.6\\
4&ABCD&0.6&FH&1.0\\
5&EGH&0.9&ABCD&1.4\\
6&EFGH&1.0&EFGH&1.5\\
7&ABCDEFGH&1.9&ABCDEFGH&3.8
\end{array}
$$

The merges at height $0.6$ may be reordered; they give the same requested three-cluster cuts. For example, the single-link distance from $AC$ to $BD$ is $\min(1.2,1.4,0.6,0.8)=0.6$, while its complete-link distance is their maximum $1.4$. After forming $EG$, its single-link distance to $H$ is $\min(0.9,1.2)=0.9$. The complete-link distance between $EG$ and $FH$ is $\max(1.2,0.9,1.5,1.2)=1.5$. Finally the closest cross-pair between $ABCD$ and $EFGH$ is $CG$ at $1.9$, while the farthest is $BF$ at $3.8$.

At three groups the partitions are therefore

$$
\boxed{\text{single linkage: }\{A,B,C,D\},\ \{E,G,H\},\ \{F\};}
$$



$$
\boxed{\text{complete linkage: }\{A,B,C,D\},\ \{E,G\},\ \{F,H\}.}
$$

**Two groups, $\{A,B,C,D\}$ and $\{E,F,G,H\}$, are more strongly supported by the merge heights.** For single linkage the three-to-two merge is at $1.0$, close to the preceding height $0.9$, whereas the two-to-one merge is delayed until $1.9$. For complete linkage the three-to-two merge at $1.5$ is close to $1.4$, whereas the final merge jumps to $3.8$. Both methods agree on the two-group partition but split its second group differently when forced to return three groups. A three-group choice is possible if required substantively, but is not particularly compelling from these dissimilarities alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
