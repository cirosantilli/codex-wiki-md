<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [objective time derivative](../../../../../../objective-time-derivative.md) transforms as a physical [tensor](../../../../../../tensor.md) under a time-dependent rigid change of observer. If $x^*=Q(t)x+c(t)$, with $Q$ orthogonal and $A^*=QAQ^T$, objectivity requires

$$
\boxed{\left(\frac{\mathcal DA}{\mathcal Dt}\right)^*
=Q\frac{\mathcal DA}{\mathcal Dt}Q^T.}
$$

This means the [constitutive equation](../../../../../../constitutive-equation.md) makes the same physical prediction in translating and rotating frames, rather than requiring individual tensor components to be invariant.

The printed plus commutator uses the derivative-index-first [velocity gradient](../../../../../../velocity-gradient.md), $G_{ij}=\partial_i u_j$. This is the transpose of the component-index-first convention $L_{ij}=\partial_j u_i$ often used for the [velocity gradient](../../../../../../velocity-gradient.md). In this notation $\omega=G-G^T$, and the rate is the [Jaumann derivative](../../../../../../jaumann-derivative.md)

$$
\frac{\mathcal DA}{\mathcal Dt}=D_tA+\frac12(\omega A-A\omega),\qquad
D_t=\partial_t+u\cdot\nabla.
$$

To check the [covariance of the Jaumann derivative](../../../../../../covariance-of-the-jaumann-derivative.md), let $R=\dot Q Q^T$. Direct transformation gives

$$
D_t^*A^*=Q(D_tA)Q^T+RA^*-A^*R,\qquad
\omega^*=Q\omega Q^T-2R.
$$

The observer-rotation terms cancel in the displayed corotational rate. Equivalently, in the $L$ convention the physical [spin tensor](../../../../../../spin-tensor.md) is $W=(L-L^T)/2=-\omega/2$, and the same rate is $D_tA-WA+AW$. One must transpose the gradient and reverse the commutator together; using $L$ in the printed plus-sign expression would not be objective.

Another example is the [upper-convected derivative](../../../../../../upper-convected-derivative.md), written consistently in the $L$ convention as

$$
\boxed{\overset{\triangledown}{A}=D_tA-LA-AL^T.}
$$

The extra terms in $L^*=QLQ^T+R$ cancel those in $D_t^*A^*$, so this also transforms covariantly. In contrast, the uncorrected [material derivative](../../../../../../material-derivative.md) $D_tA$ of a second-rank tensor is **not objective**: its transformation contains $RA^*-A^*R$. For instance a constant anisotropic tensor in a stationary fluid has zero material derivative in its original frame, but its components have a nonzero commutator derivative in a rotating observer's frame. The ordinary partial time derivative is likewise not an objective tensor rate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
