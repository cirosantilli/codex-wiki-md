<h1 id="3/e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The stated ability is a complete failure of [second-preimage resistance](../../../../../../second-preimage-resistance.md). Given an arbitrary target message $x$, compute $x'\ne x$ with $h(x')=h(x)$. Ask the signer for a [digital signature](../../../../../../digital-signature.md) on $x'$ only, obtaining $s=f(\mathit{sk},h(x'))$. Then

$$
g(\mathit{pk},s)=h(x')=h(x),
$$

so $(x,s)$ is a forgery of the chosen target. The inequality $x'\ne x$ ensures that the adversary has not requested the target's own [digital signature](../../../../../../digital-signature.md).



$$
\boxed{\text{Alternative preimages for every message give universal chosen-message forgery.}}
$$

Under a [known-message signature attack](../../../../../../known-message-signature-attack.md), the same weakness also gives an [existential forgery](../../../../../../existential-forgery.md): take an observed signed $x$, find its different second preimage, and reuse the [digital signature](../../../../../../digital-signature.md). The [universal forgery](../../../../../../universal-forgery.md) claim uses the stronger [chosen-message signature attack](../../../../../../chosen-message-signature-attack.md) capability to request the companion of whichever target was specified.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
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
