<h1 id="4h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each test divides the current candidate set into a tested subset and its complement: failure places the defective item inside the subset, whereas success places it outside. A sequence of tests is therefore a binary [decision tree](../../../../../../decision-tree.md), and minimizing its expected depth is the [Huffman coding](../../../../../../huffman-coding.md) problem with weights $1,2,\ldots,10$.

Combine the smallest two current weights repeatedly. One choice of merges is $1+2=3$, $3+3=6$, $4+5=9$, $6+6=12$, $7+8=15$, $9+9=18$, $10+12=22$, $15+18=33$, $22+33=55$. It gives this explicit [prefix code](../../../../../../prefix-code.md):

$$
\begin{array}{c|cccccccccc}
\text{item}&1&2&3&4&5&6&7&8&9&10\\\hline
\text{code}&01110&01111&0110&1110&1111&010&100&101&110&00
\end{array}
$$

At any node, test the candidate items whose next code digit is one. Assign failure to digit one and success to digit zero, and repeat until only a single codeword remains. This specifies every test, including the first subset $\{4,5,7,8,9\}$. [Huffman coding](../../../../../../huffman-coding.md) minimizes the weighted codeword lengths, so the optimal expected number is

$$
\boxed{\mathbb E[T]=\frac{173}{55}\simeq3.14545.}
$$

The sum of the successive merged weights is another check on the numerator $173$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4H](../../4h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
