<h1 id="3/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The standard attack on this raw trapdoor construction chooses a candidate [digital signature](../../../../../../digital-signature.md) $s$ first, computes $y=g(\mathit{pk},s)$, and uses a failure of [preimage resistance](../../../../../../preimage-resistance.md) to find $x$ with $h(x)=y$. Then

$$
g(\mathit{pk},s)=h(x),
$$

so $(x,s)$ verifies. The resulting message is selected by the inversion procedure, rather than being an arbitrary prescribed document. This is an [existential forgery](../../../../../../existential-forgery.md) under a [key-only signature attack](../../../../../../key-only-signature-attack.md) whenever the inversion weakness applies with nonnegligible success to those sampled digests.

$$
\boxed{\text{Invert }g(\mathit{pk},s)\text{ under }h:\ \text{existential, key-only, on covered digests}.}
$$

The phrase “fails to be preimage resistant” must be read with its target distribution. Since $g$ is a [permutation](../../../../../../permutation.md), uniform $s$ gives a uniform $n$-[bit](../../../../../../bit.md) digest; if inversion works only on a tiny identifiable exceptional set, this sampling method need not be feasible. Merely knowing a valid signed message and recovering that same message from its digest is not a new forgery. Producing a different message there requires a failure of [second-preimage resistance](../../../../../../second-preimage-resistance.md). Part [solution](../iii/solution.md) removes the coverage qualification by explicitly granting inversion at every digest.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../iii/solution.md)
