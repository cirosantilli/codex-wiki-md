<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Euclidean algorithm](../../../../../../euclidean-algorithm.md) repeatedly replaces $(r_{i-1},r_i)$ by $(r_i,r_{i-1}-q_i r_i)$, where the new remainder lies between $0$ and $r_i-1$. Common divisors are unchanged by this subtraction, and decreasing positive remainders ensure termination. The last nonzero remainder is the [greatest common divisor](../../../../../../greatest-common-divisor.md).

The [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md) also tracks coefficients $r_i=u_i a+v_i b$, beginning with coefficient pairs $(1,0)$ and $(0,1)$ and applying the same subtraction to the pairs. This invariant produces [Bézout coefficients](../../../../../../bezout-coefficient.md) for the last nonzero remainder. Here the divisions are

$$
580=2\cdot252+76,\qquad
252=3\cdot76+24,\qquad
76=3\cdot24+4,\qquad
24=6\cdot4.
$$

Back substitution gives

$$
4=76-3\cdot24=10\cdot76-3\cdot252=10\cdot580-23\cdot252.
$$

Thus **$\gcd(580,252)=4$**, with **$m=10$ and $n=-23$** in [Bézout's identity](../../../../../../bezout-s-identity.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
