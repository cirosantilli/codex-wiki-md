<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an [even integer](../../../../even-number.md) $m\geq2$, **merge the two least weights once, then repeatedly merge three least weights** until only the [tree root](../../../../root-of-a-tree.md) remains. The initial binary merge leaves an [odd number](../../../../odd-number.md) of weighted objects, so the preceding algorithm applies. The initial merged [tree parent](../../../../parent-in-a-rooted-tree.md) has two [tree children](../../../../child-in-a-rooted-tree.md); subsequent [tree parents](../../../../parent-in-a-rooted-tree.md) have three. Equivalently, add one zero-weight dummy symbol, run the odd-leaf [ternary Huffman coding](../../../../ternary-huffman-coding.md) algorithm, and remove its [codeword](../../../../codeword.md) afterwards. The dummy contributes nothing to [expected codeword length](../../../../expected-codeword-length.md).

Here the first merge joins the two weights $1/8$, producing $1/4$. The three remaining weights are $1/2,1/4,1/4$, and merge directly into the [tree root](../../../../root-of-a-tree.md). Assigning the first two [tree root](../../../../root-of-a-tree.md) branches to the original symbols of weights $1/2$ and $1/4$ gives

$$
\boxed{c(1)=0,\quad c(2)=1,\quad c(3)=20,\quad c(4)=21,\qquad L(c)=\frac54\ \text{trits}.}
$$

The merge-weight check gives $1/4+1=5/4$ as well. For $m=2$, the first merge is already the [tree root](../../../../root-of-a-tree.md); for $m=1$, outside this case with an [even number](../../../../even-number.md) of symbols, the usual temporary reduced-problem convention would permit an [empty word](../../../../empty-word.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
