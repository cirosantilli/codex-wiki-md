<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [ciphertext-only attack](../../../../../ciphertext-only-attack.md), the adversary sees [ciphertexts](../../../../../ciphertext.md) but has no supplied corresponding [plaintexts](../../../../../plaintext.md). In a [known-plaintext attack](../../../../../known-plaintext-attack.md), it also knows one or more matching [plaintext](../../../../../plaintext.md)–[ciphertext](../../../../../ciphertext.md) pairs. In a [chosen-plaintext attack](../../../../../chosen-plaintext-attack.md), it can select [plaintexts](../../../../../plaintext.md) and obtain their [encryptions](../../../../../encryption.md), possibly choosing later inputs from earlier results.

The ordinary [exhaustive key search](../../../../../exhaustive-key-search.md) is a [known-plaintext attack](../../../../../known-plaintext-attack.md): given $x$ and $c=E_k(x)$, try candidate keys $k'$ and compare $E_{k'}(x)$ with $c$. A uniformly selected $m$-[bit](../../../../../bit.md) key has average position $(2^m+1)/2$ in any fixed search order, so

$$
\boxed{\text{ordinary exhaustion: known plaintext; approximately }2^{m-1}\text{ encryptions}.}
$$

This counts testing until the actual key is reached. One known pair may leave false candidate keys when $m$ is large relative to the block length $n$; additional pairs distinguish them. If a [plaintext](../../../../../plaintext.md) has recognisable redundancy, a [ciphertext-only attack](../../../../../ciphertext-only-attack.md) can sometimes test keys by that redundancy instead, but this is an additional assumption rather than the standard supplied-pair setting.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computer security](../../../computer-security-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
