<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are three distinguishable output groups: columns $\{1,2\}$ can arise only from input one; column $\{3\}$ can arise from inputs two or three, whose rows are identical; and columns $\{4,5\}$ can arise only from input four.

Each group has zero internal [channel capacity](../../../../../channel-capacity.md). A block with one input cannot carry a variable input choice, and the middle block has identical output laws for both of its inputs. Combining the three disjoint zero-capacity blocks therefore gives

$$
\boxed{C_N=\log_2(1+1+1)=\log_2 3\text{ bits per use}.}
$$

Equivalently, the output identifies exactly which of these three groups was used, so [mutual information](../../../../../mutual-information.md) is the [entropy](../../../../../information-entropy-split.md) of that group label. It is maximized when all group [probabilities](../../../../../probability.md) are one third. The capacity-achieving input distributions are precisely

$$
p_1=p_4=\frac13,\qquad p_2+p_3=\frac13.
$$

Splitting the middle [probability](../../../../../probability.md) arbitrarily cannot communicate an extra distinction because its two [channel](../../../../../communication-channel.md) rows agree.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
