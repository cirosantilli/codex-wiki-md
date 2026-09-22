<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For encrypt-and-authenticate, the transmitted pair is $(E_k(x),s)$ with $s=f(\mathit{sk},x)$. The recovery map is public, so any observer computes

$$
\boxed{x=g(\mathit{pk},s).}
$$

No symmetric key, [exhaustive key search](../../../../../../exhaustive-key-search.md) or oracle is needed. Publishing this message-recovery [digital signature](../../../../../../digital-signature.md) reveals the entire [plaintext](../../../../../../plaintext.md) and breaks [cryptographic confidentiality](../../../../../../cryptographic-confidentiality.md) outright. A [digital signature](../../../../../../digital-signature.md) of a suitable digest would have different leakage properties, but the printed construction signs the raw block.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
