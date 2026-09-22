<h1 id="3/e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose any candidate [digital signature](../../../../../../digital-signature.md) $s$, compute $y=g(\mathit{pk},s)$, and invoke the granted algorithm to find $x$ with $h(x)=y$. Output $(x,s)$. Every chosen $s$ now leads to a valid message, with no need to search for a digest on which inversion happens to work.



$$
\boxed{\text{Every-digest inversion gives an existential forgery under key-only attack.}}
$$

This is stronger coverage than the generic failure discussed in [solution](../i/solution.md), but it does not by itself give a [universal forgery](../../../../../../universal-forgery.md). For a target message $x_*$ fixed beforehand, the adversary needs $s$ satisfying $g(\mathit{pk},s)=h(x_*)$, which inverts the trapdoor map $g$. Inverting $h$ instead produces some message for a chosen digest and does not compute that $s$.

Nor does an arbitrary preimage algorithm necessarily produce a message different from $x_*$ when invoked on $h(x_*)$: it may return $x_*$ itself. Thus a [universal forgery](../../../../../../universal-forgery.md) under a [chosen-message signature attack](../../../../../../chosen-message-signature-attack.md) needs an additional alternative-preimage guarantee, precisely the distinction supplied in [solution](../iv/solution.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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

- [Solution](../i/solution.md)
