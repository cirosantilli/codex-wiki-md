<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The final messages contain fixed greetings, rather than a fresh challenge for their particular run. Their freshness is inherited entirely from the [session key](../../../../../../session-key.md). If a key is reused, a previously recorded $E_k(\text{Hello Alice})$ or $E_k(\text{Hello Bob})$ becomes acceptable evidence again. An adversary can then mount a [replay attack](../../../../../../replay-attack.md) without knowing $k$ and without the purported speaker taking part in the new run.

Reusing a previously compromised [session key](../../../../../../session-key.md) is worse: the adversary can create both confirmations and read protected traffic. Fresh independent [session keys](../../../../../../session-key.md) limit that reuse, although they cannot fix the unauthenticated-ticket flaw shown in [solution](../i/solution.md).

$$
\boxed{\text{Fixed confirmations are fresh only when their session key is fresh.}}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
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
