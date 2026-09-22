<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Let $M(x)=ax^6+bx^5+cx^4+dx^3+ex^2+fx+g$. With [CRC generator polynomial](../../../../../crc-generator-polynomial.md) $x+1$, the appended check has one [bit](../../../../../bit.md). The preceding [polynomial remainder](../../../../../remainder-of-polynomial-division.md) rule gives $(xM)(1)=M(1)$, so put $h=a+b+c+d+e+f+g$ in the [field with two elements](../../../../../field-with-two-elements.md). The eight transmitted [bits](../../../../../bit.md) are

$$
\boxed{\langle a,b,c,d,e,f,g,\ a\mathbin\oplus b\mathbin\oplus c\mathbin\oplus d\mathbin\oplus e\mathbin\oplus f\mathbin\oplus g\rangle.}
$$

They have even [Hamming weight](../../../../../hamming-weight.md), so this [cyclic redundancy check](../../../../../cyclic-redundancy-check.md) is a [single parity-check code](../../../../../single-parity-check-code.md). For a substitution error [polynomial](../../../../../polynomial-split.md) $E$, detection occurs exactly when $E(1)=1$: an odd number of the eight [bits](../../../../../bit.md), including the check [bit](../../../../../bit.md), have flipped. Therefore

$$
\boxed{\text{every odd number of bit flips is detected; every even number is undetected}.}
$$

In particular, every single-[bit](../../../../../bit.md) error is detected, while flipping any two distinct [bits](../../../../../bit.md) passes this check. This conclusion assumes that the eight-[bit](../../../../../bit.md) word's boundaries and length are retained; it supplies no general protection against insertions, deletions or lost [framing](../../../../../framing.md).

## ↑ Ancestors (11)

1. [H](../h.md)
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
