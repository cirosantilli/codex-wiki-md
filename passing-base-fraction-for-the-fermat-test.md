# Passing-base fraction for the Fermat test

↑ **Parent:** [Carmichael number](carmichael-number.md)

Among the [units](unit-in-a-ring.md) $U(N)$ modulo $N$, the passing [residue classes](residue-class.md) form the [kernel of a group homomorphism](kernel-of-a-group-homomorphism.md) $a\mapsto a^{N-1}$. If each trial samples independently and uniformly from those [units](unit-in-a-ring.md), with replacement, the probability that $r$ trials all pass is $\alpha_N^r$. This statement assumes that sampling rule; it does not describe arbitrary or dependent choices of bases.

For $341=11\cdot31$, the [Chinese remainder theorem](chinese-remainder-theorem.md) identifies the [unit group](unit-group.md) with cyclic groups of orders $10$ and $30$. The number of solutions of $x^{340}=1$ is $\gcd(340,10)\gcd(340,30)=100$, among $\varphi(341)=300$ [units](unit-in-a-ring.md). Thus $\alpha_{341}=1/3$. The [Carmichael numbers](carmichael-number.md) $561$ and $1105$ have passing fractions $320/320$ and $768/768$, so their conditional false-pass probability remains one regardless of the number of independent trials.

<a id="image-all-nonzero-bases-coprime-passes-coprime-witnesses-and-factor-revealing-nonunits"></a>
![](fermat-test-all-base-outcome-counts.png)

**[Figure 20](#image-all-nonzero-bases-coprime-passes-coprime-witnesses-and-factor-revealing-nonunits). All nonzero bases: coprime passes, coprime witnesses and factor-revealing nonunits**. Exact enumeration for four stipulated moduli. A [greatest common divisor](greatest-common-divisor.md) check separates [nonunits](nonunit.md) before [modular exponentiation](modular-exponentiation.md). Counts are finite arithmetic results, not measured rates or a universal bound for a [primality test](primality-testing.md).

The [Fermat test example](fermat-test-example.md) uses selected bases; this diagram exhausts the specified finite base sets. Both make the same logical distinction: an exponent witness can prove compositeness, whereas a passing result needs further justification before it can support a claim of primality.

## ↑ Ancestors (5)

1. [Carmichael number](carmichael-number.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Carmichael number](carmichael-number.md)
