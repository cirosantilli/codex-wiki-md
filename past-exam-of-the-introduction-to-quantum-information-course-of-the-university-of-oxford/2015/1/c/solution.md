<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An observed value $k$ must lie in the [image](../../../../image-of-a-function.md) of $f$. Choose either [preimage](../../../../preimage.md) $x_k$. The [two-to-one function](../../../../two-to-one-function.md) promise and $s\ne0^n$ imply that its [preimages](../../../../preimage.md) are exactly $x_k$ and $x_k\oplus s$. A [computational-basis measurement](../../../../quantum-measurement-in-the-computational-basis.md) of the second [quantum register](../../../../quantum-register.md) projects the joint [quantum state](../../../../quantum-state.md) onto the unnormalized vector

$$
2^{-n/2}\bigl(|x_k\rangle+|x_k\oplus s\rangle\bigr)|k\rangle.
$$

By the [Born rule](../../../../born-rule.md), $\Pr(k)=2^{1-n}$. Dividing by its square root gives the conditional first-register [pure state](../../../../pure-state.md)

$$
\boxed{|\psi_k\rangle=\frac{|x_k\rangle+|x_k\oplus s\rangle}{\sqrt2}.}
$$

Choosing the other [preimage](../../../../preimage.md) merely interchanges the two summands. The result is a [Simon coset state](../../../../simon-coset-state.md), retaining [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md) between the two inputs that share the measured function value. Outcomes outside the [image](../../../../image-of-a-function.md) have [probability](../../../../probability.md) zero and hence no conditional state to normalize.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
