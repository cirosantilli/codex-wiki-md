<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Represent the data [bits](../../../../../bit.md), most significant first, by a [polynomial](../../../../../polynomial-split.md) $M(x)$ whose [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md) lie in the [field with two elements](../../../../../field-with-two-elements.md) $\mathbb F_2$. Here [addition](../../../../../addition.md) and [subtraction](../../../../../subtraction.md) are both [exclusive or](../../../../../exclusive-or.md), with no carries. Choose a fixed [CRC generator polynomial](../../../../../crc-generator-polynomial.md) $G(x)$ of [polynomial degree](../../../../../degree-of-a-polynomial.md) $r$, with leading and constant [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md) one. Both [endpoints](../../../../../communication-endpoint.md) know $G$ and the [bit](../../../../../bit.md) ordering.

Multiply $M$ by $x^r$, which appends $r$ zero [bits](../../../../../bit.md). Use [polynomial division](../../../../../polynomial-division.md) to obtain

$$
x^rM(x)=Q(x)G(x)+R(x),\qquad R=0\ \text{or}\ \deg R<r.
$$

Replace the appended zeros by the $r$ [bits](../../../../../bit.md) of the [polynomial remainder](../../../../../remainder-of-polynomial-division.md) $R$, retaining leading zeros when necessary. The transmitted [polynomial](../../../../../polynomial-split.md) is

$$
\boxed{T(x)=x^rM(x)+R(x),\qquad T(x)\bmod G(x)=0.}
$$

The last equality holds because adding $R$ cancels the existing [polynomial remainder](../../../../../remainder-of-polynomial-division.md) in the [field with two elements](../../../../../field-with-two-elements.md). It is the simple systematic [cyclic redundancy check](../../../../../cyclic-redundancy-check.md) convention used here; practical variants can add agreed initialization and final transformations.

The receiver divides the entire received [polynomial](../../../../../polynomial-split.md) by $G$. A nonzero [polynomial remainder](../../../../../remainder-of-polynomial-division.md) detects corruption. If the received word is $T+E$, where the ones in the error [polynomial](../../../../../polynomial-split.md) $E$ mark flipped [bits](../../../../../bit.md), its [polynomial remainder](../../../../../remainder-of-polynomial-division.md) is $E\bmod G$. Thus the undetected nonzero errors are exactly the multiples of $G$; a zero result does not prove that transmission was error-free. Operationally, [polynomial long division](../../../../../polynomial-long-division.md) repeatedly cancels a leading one using a shifted copy of $G$, implemented with [exclusive or](../../../../../exclusive-or.md) operations.

## ↑ Ancestors (11)

1. [F](../f.md)
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
