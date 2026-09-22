<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Complete the square to obtain the equivalent [quadratic congruence](../../../../quadratic-congruence.md)

$$
(x+3)^2\equiv1111\pmod{8093}.
$$

Here $\gcd(1111,8093)=1$: the [Euclidean algorithm](../../../../euclidean-algorithm.md) has successive nonzero remainders $316,163,153,10,3,1$. If this [modular congruence](../../../../modular-congruence.md) had a solution, the [Jacobi symbol](../../../../jacobi-symbol.md) $(1111/8093)$ would be $1$, since a square [coprime](../../../../coprime-integers.md) to an odd modulus has [Legendre symbol](../../../../legendre-symbol.md) $1$ at every [prime factor](../../../../prime-factor.md). Calculate instead, using [Jacobi reciprocity](../../../../jacobi-reciprocity-law.md) and reduction of numerators,

$$
\begin{aligned}
\left(\frac{1111}{8093}\right)
&=\left(\frac{8093}{1111}\right)&& (8093\equiv1\pmod4)\\
&=\left(\frac{316}{1111}\right)&& (8093=7\cdot1111+316)\\
&=\left(\frac4{1111}\right)\left(\frac{79}{1111}\right)=\left(\frac{79}{1111}\right)\\
&=-\left(\frac{1111}{79}\right)&& (79\equiv1111\equiv3\pmod4)\\
&=-\left(\frac5{79}\right)&& (1111=14\cdot79+5)\\
&=-\left(\frac{79}5\right)=-\left(\frac45\right)=-1.
\end{aligned}
$$

Therefore **there is no solution**. This obstruction does not require a separate primality test for $8093$; the [Jacobi symbol](../../../../jacobi-symbol.md) suffices.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
