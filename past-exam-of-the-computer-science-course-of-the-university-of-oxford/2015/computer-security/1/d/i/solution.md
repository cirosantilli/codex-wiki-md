<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Avoid constructing the huge [integers](../../../../../../integer-split.md) $c^{3^j}$ explicitly. Maintain $a_0=c$ and $a_j=a_{j-1}^3\bmod n$, computing $g_j=\gcd(a_j-c,n)$ after each step.

In case (1), the nontrivial [greatest common divisor](../../../../../../greatest-common-divisor.md) $g_k$ is one of the [prime factors](../../../../../../prime-factor.md) $p,q$. Divide $n$ by it, compute $d$ with the [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md), and return $c^d\bmod n$.

In case (2), $a_k=c\pmod n$. The preceding value satisfies $a_{k-1}^3=c\pmod n$. Cubing is a [bijection](../../../../../../bijection.md) on the [residue classes](../../../../../../residue-class.md) modulo $n$, so there is only one such cube root, namely the original [plaintext](../../../../../../plaintext.md) $m$. Therefore

$$
\boxed{\begin{array}{ll}1<g_k<n:&\text{factor }n\text{ and decrypt};\\g_k=n:&m=a_{k-1}=c^{3^{k-1}}\bmod n.\end{array}}
$$

For $k=1$, the preceding value is $a_0=c$; a fixed point is its own [plaintext](../../../../../../plaintext.md). Keeping the previous iterate makes the recovery immediate once the [RSA cycling attack](../../../../../../rsa-cycling-attack.md) succeeds.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
