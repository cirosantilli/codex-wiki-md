<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For encrypt-then-authenticate, choose any $n$-[bit](../../../../../../bit.md) string $s$ and compute

$$
c=g(\mathit{pk},s).
$$

Send $(c,s)$. The receiver's correct check for this composition is $g(\mathit{pk},s)=c$ before [decryption](../../../../../../decryption.md), so it passes by construction. The receiver obtains a [plaintext](../../../../../../plaintext.md) $x=D_k(c)$, although the adversary may not know it.

The finite domains justify the signature relation: $g\circ f$ is the identity on $2^n$ messages, so $f$ is injective and therefore bijective. Hence $g=f^{-1}$ and also $f\circ g$ is the identity. The chosen $s$ is therefore exactly $f(\mathit{sk},c)$, without the adversary ever evaluating $f$.

$$
\boxed{(g(\mathit{pk},s),s)\text{ is an existential forgery.}}
$$

This is a [key-only signature attack](../../../../../../key-only-signature-attack.md) against raw unrestricted trapdoor signing. It does not invert $g$ at a chosen target and does not contradict the assumption that signing an independently specified new message is hard. It exploits choosing the [digital signature](../../../../../../digital-signature.md) first. The observation concerns the paper's raw construction, rather than every encrypt-then-authenticate scheme.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
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
