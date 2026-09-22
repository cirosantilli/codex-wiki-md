<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Perfect secrecy](../../../../../../perfect-secrecy.md) means that observing the [ciphertext](../../../../../../ciphertext.md) changes no [probability](../../../../../../probability.md) concerning the [plaintext](../../../../../../plaintext.md). For every distribution of the message $X$, and every $x,c$ with $\Pr(C=c)>0$,

$$
\boxed{\Pr(X=x\mid C=c)=\Pr(X=x).}
$$

Equivalently, for every pair $x,x'$ the conditional [probability distributions](../../../../../../probability-distribution-split.md) of the [ciphertext](../../../../../../ciphertext.md) are identical:

$$
\Pr(C=c\mid X=x)=\Pr(C=c\mid X=x').
$$

The randomness here comes from independent key generation and any [encryption](../../../../../../encryption.md) randomness. The claim is information theoretic: unlimited computation cannot extract information about $X$ from $C$ beyond what was known beforehand.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
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
