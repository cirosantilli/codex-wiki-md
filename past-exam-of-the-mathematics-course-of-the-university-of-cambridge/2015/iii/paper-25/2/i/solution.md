<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [immune set](../../../../../../immune-set.md) is an infinite set containing no infinite [computably enumerable](../../../../../../recursively-enumerable-set.md) subset. For [binary strings](../../../../../../binary-string.md), use an effective [bijection](../../../../../../bijection.md) with [natural numbers](../../../../../../natural-number.md) when discussing enumeration. Fix an [optimal description machine](../../../../../../optimal-description-machine.md) $U$ and define the [plain Kolmogorov complexity](../../../../../../plain-kolmogorov-complexity.md)

$$
C_U(\sigma)=\min\{|p|:U(p)=\sigma\}.
$$

An [incompressible string](../../../../../../incompressible-string.md) has no description shorter than itself, that is, $C_U(\sigma)\geq|\sigma|$. The choice of machine is fixed throughout the proof.

Let $I$ be the set of [incompressible strings](../../../../../../incompressible-string.md). There are $2^n$ strings of length $n$, but only $1+2+\cdots+2^{n-1}=2^n-1$ programs of length less than $n$. Each halting program describes at most one string, so at least one string of each length belongs to $I$. Consequently $I$ is infinite.

Suppose an infinite [computably enumerable set](../../../../../../recursively-enumerable-set.md) $E$ were contained in $I$. Define a [total computable function](../../../../../../total-computable-function.md) $q(n)$ by running an enumeration of $E$ until a string of length at least $n$ appears, and outputting the first such string. This search always terminates because there are only finitely many [binary strings](../../../../../../binary-string.md) of bounded length. A fixed program can reconstruct $q(n)$ from a [self-delimiting binary code](../../../../../../self-delimiting-binary-code.md) of $n$. For example, if the binary expansion of $n$ has length $\ell$, encode it using $\ell$ copies of one, a zero separator, and its $\ell$ binary digits. This gives

$$
C_U(q(n))\leq2\lceil\log_2(n+1)\rceil+c
$$

for a constant $c$ depending on the enumeration algorithm and the [optimal description machine](../../../../../../optimal-description-machine.md), not on $n$. For sufficiently large $n$ this is less than $n\leq|q(n)|$, contradicting $q(n)\in I$. Thus **the set of [incompressible strings](../../../../../../incompressible-string.md) is an [immune set](../../../../../../immune-set.md)**. This proves [immunity of incompressible strings](../../../../../../immunity-of-incompressible-strings.md). The argument uses the ability to describe a selected long string by the short threshold specifying how it was selected.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
