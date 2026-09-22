<h1 id="4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose $0<\theta<\pi/2$ with $\sin\theta=\sqrt p$. Then $1-2p=\cos2\theta$ and $2\sqrt{p(1-p)}=\sin2\theta$. The [matrix](../../../../../../matrix.md) found in part 2 is a rotation by $2\theta$ in the ordered good-bad plane, with the bad coordinate listed first. The initial coordinate vector is $(\cos\theta,\sin\theta)^T$.

After $r$ rotations its angle from the bad axis is $(2r+1)\theta$. Equivalently, multiplication of the displayed [matrix](../../../../../../matrix.md) and the addition formulas for sine and cosine prove the assertion by induction from $r=0$. Hence

$$
\boxed{Q^r|\Psi\rangle=\cos((2r+1)\theta)|b\rangle+\sin((2r+1)\theta)|g\rangle.}
$$

The [Born rule](../../../../../../born-rule.md) therefore gives good-output probability $\sin^2((2r+1)\theta)$. This is the geometric mechanism of [amplitude amplification](../../../../../../amplitude-amplification.md): each coherent iteration rotates the already existing good amplitude toward the good axis.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
