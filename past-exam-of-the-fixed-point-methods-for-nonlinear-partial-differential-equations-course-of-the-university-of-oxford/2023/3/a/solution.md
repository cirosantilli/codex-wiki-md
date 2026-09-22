<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A useful form of [Minty's lemma](../../../../minty-s-lemma.md) is the following. Let $X$ be a real [Banach space](../../../../banach-space-split.md), $K\subset X$ a nonempty [convex set](../../../../convex-set-split.md), and $A:K\to X^*$ a [monotone operator](../../../../monotone-operator.md) that is [hemicontinuous](../../../../hemicontinuity.md). Here [operator monotonicity](../../../../operator-monotonicity.md) means $\langle Ax-Ay,x-y\rangle\geq0$ for $x,y\in K$, and [hemicontinuity](../../../../hemicontinuity.md) means that $t\mapsto\langle A(x+t(y-x)),z\rangle$ is continuous on $[0,1]$ for $x,y\in K$ and $z\in X$. For $u\in K$,

$$
\boxed{\langle Au,v-u\rangle\geq0\ \forall v\in K
\quad\Longleftrightarrow\quad
\langle Av,v-u\rangle\geq0\ \forall v\in K.}
$$

The forward implication follows from [operator monotonicity](../../../../operator-monotonicity.md):

$$
\langle Av,v-u\rangle
=\langle Au,v-u\rangle+\langle Av-Au,v-u\rangle\geq0.
$$

For the reverse implication, fix $w\in K$ and take $v_t=u+t(w-u)\in K$ for $0<t\leq1$. The assumed inequality gives

$$
0\leq\langle Av_t,v_t-u\rangle=t\langle A(u+t(w-u)),w-u\rangle.
$$

Divide by $t$ and send $t\downarrow0$. [Hemicontinuity](../../../../hemicontinuity.md) gives $\langle Au,w-u\rangle\geq0$, as required.

In the whole-space version, for a [monotone operator](../../../../monotone-operator.md) $A:X\to X^*$ that is [hemicontinuous](../../../../hemicontinuity.md),

$$
\boxed{Au=f\quad\Longleftrightarrow\quad
\langle Av-f,v-u\rangle\geq0\quad\forall v\in X.}
$$

Apply the just-proved result to $A-f$ and $K=X$; the resulting inequality $\langle Au-f,v-u\rangle\geq0$ for all $v$ forces $Au=f$ by choosing $v=u\pm z$. This is the [variational inequality](../../../../variational-inequality.md) form of [Minty's lemma](../../../../minty-s-lemma.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
