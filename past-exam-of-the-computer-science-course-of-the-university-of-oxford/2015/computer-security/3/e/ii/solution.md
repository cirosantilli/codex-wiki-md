<h1 id="3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A failure of [collision resistance](../../../../../../collision-resistance.md) supplies distinct messages $x,x'$ with

$$
h(x)=h(x').
$$

Ask the legitimate signer to sign $x$, obtaining $s=f(\mathit{sk},h(x))$. Output $(x',s)$ without ever requesting a [digital signature](../../../../../../digital-signature.md) on $x'$. Its verification succeeds because

$$
g(\mathit{pk},s)=h(x)=h(x').
$$

Thus

$$
\boxed{\text{Collision finding gives an existential forgery under chosen-message attack.}}
$$

The adversary chooses the collision pair, but cannot in general insist that one member equal an independently specified target. A [known-message signature attack](../../../../../../known-message-signature-attack.md) would require the stronger ability to collide with an already signed message; finding an arbitrary collision alone does not provide that.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
