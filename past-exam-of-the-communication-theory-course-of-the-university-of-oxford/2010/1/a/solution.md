<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A binary code assigns a finite bit string to each source symbol. Use nonempty codewords for an unframed variable-length stream. The code is [uniquely decodable](../../../../decipherable-code.md) if no two distinct finite sequences of source symbols produce the same concatenated bit string. It is a [prefix-free code](../../../../prefix-code.md) if no [codeword](../../../../codeword.md) is an initial segment of a different [codeword](../../../../codeword.md).

To prove unique decoding of a [prefix code](../../../../prefix-code.md), suppose two concatenations agree. Their first codewords both begin the same bit string, so the shorter is a prefix of the longer. The prefix condition forces the first codewords to be equal. Cancel them and repeat. Since the codewords are nonempty, this process ends with both symbol sequences exhausted at the same time; otherwise a nonempty remainder could not equal the empty string. Hence the source sequences agree.

The code $\{0,01\}$ is not a [prefix code](../../../../prefix-code.md), since $0$ is a prefix of $01$. Nevertheless it is [uniquely decodable](../../../../decipherable-code.md): decode from the right. A final $1$ forces the last [codeword](../../../../codeword.md) to be $01$, whereas a final $0$ forces it to be $0$. Removing that final word recursively gives a unique parsing. Thus **the converse fails**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
