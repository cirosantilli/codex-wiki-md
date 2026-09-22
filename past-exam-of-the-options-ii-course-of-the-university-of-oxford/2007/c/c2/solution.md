<h1 id="c/c2/solution">Solution</h1>

↑ **Parent:** [C2](../c2.md)

[Wilson's theorem](../../../../wilson-s-theorem.md) states that for a prime $p$, $(p-1)!\equiv-1\pmod p$. For odd $p$, pair each nonzero [residue](../../../../residue.md) with its multiplicative inverse. Only the self-inverse residues remain unpaired; $x^2=1$ in a field gives $x=\pm1$. Their product is $-1$, proving the result. For $p=2$ the assertion is immediate.

If composite $n\ge6$ is not the square of a prime, choose a prime divisor $p$ such that $p$ and $n/p$ are distinct. Both occur among the factors of $(n-1)!$, so their product $n$ divides it. In the remaining case $n=p^2$, $p\ge3$, and the two distinct factors $p,2p$ both occur in the factorial and have product divisible by $p^2$. Thus the factorial is zero modulo every such composite $n$.

For prime $n$, Wilson's congruence makes the numerator sine squared equal $\sin^2(\pi/n)$, so its ratio is one. For composite $n\ge6$, the numerator vanishes. The only exceptional composite in the sum is four; its ratio is $\sin^2(3\pi/2)/\sin^2(\pi/4)=2$. Therefore for $x\ge4$ the sum counts the primes plus two, and subtracting two gives exactly the required prime count. All statements concern the integers $2\le n\le\lfloor x\rfloor$.

## ↑ Ancestors (12)

1. [C2](../c2.md)
2. [C](../../c.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
