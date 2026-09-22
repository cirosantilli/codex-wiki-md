<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The printed word “even” conflicts with the displayed numbers: all ten listed [prime numbers](../../../../../prime-number-split.md) are odd, and $2$ is the only even [prime number](../../../../../prime-number-split.md). The scan confirms that wording.[Printed p. 5, Question 9(b), both occurrences of “even” and the final “including 2”](../../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-examination-paper-by-the-university-of-oxford-2005.md) We first construct the detector for the explicitly listed numbers, then add $2$ as requested. The literal even-prime detector is also given below.

Let the five input [bits](../../../../../bit.md) be $A,B,C,D,E$ with value $16A+8B+4C+2D+E$. Every listed number has $E=1$. For that plane, the four-variable [Karnaugh map](../../../../../karnaugh-map.md) is

| $AB\backslash CD$ | $00$ | $01$ | $11$ | $10$ |
| --- | --- | --- | --- | --- |
| $00$ | $0$ | $1$ | $1$ | $1$ |
| $01$ | $0$ | $1$ | $0$ | $1$ |
| $11$ | $0$ | $0$ | $1$ | $1$ |
| $10$ | $1$ | $1$ | $1$ | $0$ |

The entire $E=0$ plane is zero. Five valid groups in the displayed [Karnaugh map](../../../../../karnaugh-map.md) give the product terms

$$
\overline A\,\overline C D,\quad
\overline A C\overline D,\quad
A\overline B\,\overline C,\quad
ABC,\quad
\overline B D.
$$

Including $E$, their accepted numbers are respectively $\{3,11\}$, $\{5,13\}$, $\{17,19\}$, $\{29,31\}$, and $\{3,7,19,23\}$. Their union is exactly the ten listed numbers. Hence an explicit [Boolean circuit](../../../../../boolean-circuit.md) is: invert $A,B,C,D$ where needed, feed the five products into five [AND gates](../../../../../and-gate.md), combine those outputs with an [OR gate](../../../../../or-gate.md), and AND with $E$. Its output is

$$
\boxed{P_{\mathrm{odd}}=E\bigl(
\overline A\,\overline C D\lor
\overline A C\overline D\lor
A\overline B\,\overline C\lor
ABC\lor\overline B D\bigr).}
$$

Any gate with more than two inputs can be replaced by a tree of two-input gates. To include the exceptional [prime number](../../../../../prime-number-split.md) $2$, detect its exact [binary representation](../../../../../binary-number.md) $00010$ and add one OR branch:

$$
\boxed{P_{\mathrm{all}}=P_{\mathrm{odd}}\lor
\overline A\,\overline B\,\overline C D\overline E.}
$$

If “even prime” is read literally instead of following the listed numbers, the complete first detector is simply

$$
\boxed{P_{\mathrm{even}}=\overline A\,\overline B\,\overline C D\overline E.}
$$

All three formulas classify all $32$ possible inputs, including $0$ and $1$ as nonprime.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
