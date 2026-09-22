<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A good item must exist, so assume $1\le k<N$; if $k=0$, the requested search is impossible, while $k=N$ makes every output good. Put $p=k/N$ and $\theta=\arcsin\sqrt p$. Normalize the good and bad components of the [uniform superposition state](../../../../../../uniform-superposition-state.md) as

$$
|g\rangle=\frac1{\sqrt k}\sum_{f(x)=1}|x\rangle,\qquad|b\rangle=\frac1{\sqrt{N-k}}\sum_{f(x)=0}|x\rangle,\qquad|\psi_0\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle.
$$

The [Boolean phase oracle](../../../../../../marked-state-phase-oracle.md) negates $|g\rangle$ and fixes $|b\rangle$. The [Grover diffusion operator](../../../../../../grover-diffusion-operator.md) is $-I_{\psi_0}=2|\psi_0\rangle\langle\psi_0|-I$. Its implementation is independent of $f$: conjugate the reflection about $|0^n\rangle$ by [Hadamard gates](../../../../../../hadamard-gate.md). One [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration is

$$
G=-I_{\psi_0}I_f=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}_{g,b}.
$$

Hence, by the [Grover rotation angle](../../../../../../grover-rotation-angle.md) formula,

$$
G^j|\psi_0\rangle=\sin((2j+1)\theta)|g\rangle+\cos((2j+1)\theta)|b\rangle.
$$

Choose the nonnegative integer $j$ nearest to $\pi/(4\theta)-1/2$. Its final angle differs from $\pi/2$ by at most $\theta$, so a [computational-basis measurement](../../../../../../quantum-measurement-in-the-computational-basis.md) succeeds with probability at least $\cos^2\theta=1-p$. The allowed small-density regime includes $p\le1/3$, giving the requested $2/3$ bound. Each iteration uses one [Boolean phase oracle](../../../../../../marked-state-phase-oracle.md) query, and $j=O(1/\sqrt p)=O(\sqrt{N/k})$.

For $k=N/4$, $\theta=\pi/6$ and one iteration reaches $3\theta=\pi/2$ exactly. **Thus one query gives a good outcome with certainty:**

$$
\boxed{G|\psi_0\rangle=|g\rangle\quad(k=N/4).}
$$

This is [exact Grover search on four entries](../../../../../../exact-grover-search-on-four-entries.md) applied to a marked fraction of one quarter, not only to a four-element register.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
