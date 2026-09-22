<h1 id="3i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [cipher](../../../../../../cipher.md) has [perfect secrecy](../../../../../../perfect-secrecy.md) when the [conditional probability](../../../../../../conditional-probability.md) of every plaintext given a ciphertext equals its prior probability: $\Pr(M=m\mid C=c)=\Pr(M=m)$ whenever $\Pr(C=c)>0$. Equivalently, the plaintext and ciphertext are [independent random variables](../../../../../../independent-random-variables.md).

Fix a ciphertext $c$ that can occur. Perfect secrecy requires every possible plaintext $m$ to remain possible after observing $c$. For a deterministic decryption rule, two different plaintexts producing $c$ require two different keys, so the key space has cardinality at least that of the message space.

In a [one-time pad](../../../../../../one-time-pad.md), the message and key belong to the same finite [additive group](../../../../../../additive-group.md), the key is [uniform](../../../../../../continuous-uniform-distribution.md) and independent of the message, and encryption is $C=M+K$. For every $m,c$ there is exactly one key $k=c-m$, so

$$
\Pr(C=c\mid M=m)=\Pr(K=c-m)=\frac1{|\mathcal K|},
$$

independent of $m$. [Bayes' theorem](../../../../../../bayes-theorem.md) then gives $\Pr(M=m\mid C=c)=\Pr(M=m)$, proving [perfect secrecy](../../../../../../perfect-secrecy.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3I](../../3i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
