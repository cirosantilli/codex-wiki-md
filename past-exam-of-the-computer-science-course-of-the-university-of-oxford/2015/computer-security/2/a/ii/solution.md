<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [trusted third party](../../../../../../trusted-third-party.md) is an additional participant whose correct behaviour and protection of its secret state are assumptions on which the other parties rely. Here Alice and Bob rely on Tim to associate identities with the right [public keys](../../../../../../public-key.md), generate fresh [session keys](../../../../../../session-key.md), and keep the long-term shared secrets confidential.

Tim is allowed to know $k_{AB}$, so the intended [cryptographic confidentiality](../../../../../../cryptographic-confidentiality.md) claim excludes the network adversary, rather than excluding Tim. Correct behaviour by Tim does not make every message purportedly sent by Tim authentic: the recipients must still verify the relevant evidence.

$$
\boxed{\text{Tim's correctness and secrecy are explicit trust assumptions.}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
