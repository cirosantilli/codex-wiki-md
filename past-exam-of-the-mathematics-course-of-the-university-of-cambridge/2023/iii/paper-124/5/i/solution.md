<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A property $\mathcal P=(\mathcal P_n)$ of $n$-variable Boolean functions is:

- [constructive](../../../../../../constructive-property-of-boolean-functions.md) if membership can be decided from the $2^n$-bit truth table in time polynomial in $2^n$;
- [large](../../../../../../large-property-of-boolean-functions.md) if a uniformly random Boolean function belongs to $\mathcal P_n$ with probability at least $2^{-O(n)}$;
- [useful](../../../../../../useful-property-against-a-circuit-class.md) against a circuit class $\mathcal C$ if infinitely often $\mathcal P_n$ contains a function but contains no function computed by circuits in $\mathcal C$ of the target size.

A property satisfying all three conditions is a [natural proof](../../../../../../natural-proof.md). The [Razborov–Rudich natural-proofs barrier](../../../../../../razborov-rudich-natural-proofs-barrier.md) states that if exponentially secure [pseudorandom function families](../../../../../../pseudorandom-function-family.md) exist in $\mathrm{P}/\mathrm{poly}$, then no property that is constructive and large is useful against polynomial-size circuits.

Suppose such a property $\mathcal P$ existed. Given oracle access to an unknown $n$-variable function, query its full truth table and run the constructive membership test. This takes $2^{O(n)}$ time. For a truly random function, largeness makes the test accept with probability at least $2^{-O(n)}$. Repetition amplifies this to a constant acceptance probability within $2^{O(n)}$ time.

For a function drawn from the assumed pseudorandom family, each keyed function has polynomial-size circuits, so usefulness makes the test reject for the relevant lengths. The amplified membership test therefore distinguishes the pseudorandom family from a truly random function with constant advantage in exponential time, contradicting exponential pseudorandomness. Hence the three conditions cannot coexist.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
