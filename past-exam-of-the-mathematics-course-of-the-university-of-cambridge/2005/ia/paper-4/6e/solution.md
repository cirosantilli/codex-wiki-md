<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

An [equivalence relation](../../../../../equivalence-relation.md) is [reflexive](../../../../../reflexive-relation.md), [symmetric](../../../../../symmetric-relation.md) and [transitive](../../../../../transitive-relation.md): for all $a,b,c\in S$, one has $aRa$; $aRb$ implies $bRa$; and $aRb$, $bRc$ imply $aRc$. Define the [equivalence class](../../../../../equivalence-class.md) $[a]=\{b\in S:aRb\}$. Reflexivity puts $a$ in its class, so these classes cover $S$ and are nonempty. If $[a]$ and $[b]$ share $c$, symmetry and transitivity give $aRb$; the same properties show that every element of either class is in the other. Thus two classes are equal or disjoint. **The distinct equivalence classes form a partition of the set.**

For the relation defined by a [subgroup](../../../../../subgroup.md) $H\le G$, $a^{-1}a=1\in H$ proves reflexivity. If $a^{-1}b\in H$, its inverse $b^{-1}a$ belongs to $H$, proving symmetry. If also $b^{-1}c\in H$, their product is $a^{-1}c\in H$, proving transitivity. Finally,

$$
[a]=\{b:a^{-1}b\in H\}=aH.
$$

These are exactly the left [cosets](../../../../../coset.md). The map $H\to gH$, $h\mapsto gh$, is a [bijection](../../../../../bijection.md), with inverse $x\mapsto g^{-1}x$. If $G$ is finite and has $r$ such [cosets](../../../../../coset.md), their disjoint union gives $|G|=r|H|$. This proves the [Lagrange theorem](../../../../../lagrange-s-theorem.md):

$$
\boxed{|H|\mid|G|.}
$$

For $g\in G$, finitely many possible powers imply $g^a=g^b$ for some $a<b$, so a positive power is the [identity element](../../../../../identity-element.md). If its least positive exponent is $n$, the powers $1,g,\ldots,g^{n-1}$ are distinct: equality of two would produce a smaller positive exponent. They are closed under products and inverses by reducing exponents modulo $n$, hence form the [cyclic subgroup](../../../../../cyclic-subgroup.md) $\langle g\rangle$ of cardinality $n$. The [Lagrange theorem](../../../../../lagrange-s-theorem.md) gives $n\mid|G|$, and consequently

$$
\boxed{g^{|G|}=1\quad\text{for every }g\in G.}
$$

Now take a positive modulus $m$. On residue classes modulo $m$, consider the classes with representatives [coprime](../../../../../coprime-integers.md) to $m$. The following integer facts are used: multiplication is associative; reducing representatives respects products; a prime dividing a product divides a factor; and the [Bezout identity](../../../../../bezout-identity.md) gives $ra+sm=1$ when $\gcd(a,m)=1$. If $a,b$ are coprime to $m$, no prime divisor of $m$ divides $ab$, so their product class is again in the set. The class of $1$ is its [identity element](../../../../../identity-element.md). The Bézout equation gives $ra\equiv1\pmod m$, and $r$ is also coprime to $m$ because any common divisor of $r,m$ would divide $1$. Thus every class has an inverse, and these classes form the [group of units modulo an integer](../../../../../multiplicative-group-of-integers-modulo-n.md).

Representing classes in $\{1,\ldots,m\}$ gives precisely the group in the question; for $m=1$ this is the one-element group. Its cardinality is the [Euler totient function](../../../../../euler-totient-function.md) $\varphi(m)$. Applying the finite-group exponent result yields the [Fermat-Euler theorem](../../../../../euler-s-theorem.md):

$$
\boxed{a^{\varphi(m)}\equiv1\pmod m\qquad\text{if }\gcd(a,m)=1.}
$$

For $m=1$ the congruence is automatic.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
