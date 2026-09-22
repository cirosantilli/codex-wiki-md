<h1 id="c/c1/solution">Solution</h1>

↑ **Parent:** [C1](../c1.md)

Use the agreed text encoding to split the plaintext into integer blocks $m_j\in\{0,\ldots,1072\}$. [RSA](../../../../rsa-cryptosystem.md) encrypts each block by [modular exponentiation](../../../../modular-exponentiation.md):

$$
r_j\equiv m_j^{11}\pmod{1073}.
$$

Because $1073=29\cdot37$ is a product of distinct [primes](../../../../prime-number-split.md), its [Euler totient function](../../../../euler-totient-function.md) is $\varphi(1073)=28\cdot36=1008$. The inverse exponent follows from

$$
11\cdot275=3025=1+3\cdot1008.
$$

Thus **a decryption exponent is 275**, and the three recovered blocks are

$$
\boxed{m_j\equiv r_j^{275}\pmod{1073},\quad0\leq m_j<1073,\quad j=1,2,3}.
$$

To check every block, including blocks not [coprime](../../../../coprime-integers.md) to the modulus, reduce modulo each prime. If $m_j$ is nonzero modulo 29, [Fermat's little theorem](../../../../fermat-little-theorem.md) gives $m_j^{3025}=m_j$ because $28\mid3024$; if it is zero the equality is immediate. The same argument works modulo 37 because $36\mid3024$. The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) then gives the equality modulo 1073. Finally reverse the agreed text encoding. The symbols $r_1,r_2,r_3$ are unspecified, so there are no numerical message blocks to evaluate further.

## ↑ Ancestors (12)

1. [C1](../c1.md)
2. [C](../../c.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
