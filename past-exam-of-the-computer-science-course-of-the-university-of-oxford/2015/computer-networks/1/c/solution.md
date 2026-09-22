<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [block code for line coding](../../../../../block-code-for-line-coding.md) divides the data into five-[bit](../../../../../bit.md) groups and assigns each of the $2^5=32$ possible groups a distinct eight-[bit](../../../../../bit.md) [codeword](../../../../../codeword.md). The receiver reverses that assignment after finding the eight-[bit](../../../../../bit.md) boundaries. There are $2^8=256$ candidate [codewords](../../../../../codeword.md), so the designer has substantial freedom to select 32 suitable ones and reserve other patterns for control or synchronization.

The choice can limit long runs of equal [bits](../../../../../bit.md) to help [clock recovery](../../../../../clock-recovery.md), balance high and low levels to reduce a persistent offset, and distinguish control patterns from data. These properties must hold across adjacent [codeword](../../../../../codeword.md) boundaries too: two individually acceptable words can concatenate into an unacceptable run. The unused patterns can also help [error detection and correction](../../../../../error-detection-and-correction.md): an invalid received pattern exposes some errors, and the [Hamming distance](../../../../../hamming-distance.md) between valid [codewords](../../../../../codeword.md) determines stronger guarantees. Redundancy alone does not imply that all errors are detected or correctable. Circuit complexity and propagation of a synchronization error also matter.

Before any further [line coding](../../../../../line-code.md) or [framing](../../../../../framing.md) overhead, the useful fraction and expansion are

$$
\boxed{\text{useful fraction}=\frac58=62.5\%,\qquad \text{transmitted bits per data bit}=\frac85.}
$$

The three extra [bits](../../../../../bit.md) per five input [bits](../../../../../bit.md) are 60% overhead relative to the input, or 37.5% of the encoded output.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
