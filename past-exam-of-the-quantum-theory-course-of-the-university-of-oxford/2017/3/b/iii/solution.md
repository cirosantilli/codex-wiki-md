<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Recover $L_1$ from the given [angular momentum raising operator](../../../../../angular-momentum-raising-operator.md) and [angular momentum lowering operator](../../../../../angular-momentum-lowering-operator.md):

$$
L_1=\frac12(L_++L_-)=i\hbar\left(\sin\phi\,\partial_\theta+\cot\theta\cos\phi\,\partial_\phi\right).
$$

This is the generator of [rotations](../../../../../rotation-mathematics.md) about the first coordinate axis. A natural candidate is the angular function pointing along that axis, $f_x=\sin\theta\cos\phi$. Direct substitution gives

$$
L_1f_x=i\hbar\left(\sin\phi\cos\theta\cos\phi-\cot\theta\cos\phi\sin\theta\sin\phi\right)=0.
$$

Also $f_x=(f_{+1}+f_{-1})/2$, so [linearity](../../../../../linearity.md) and part (ii) give $L^2f_x=2\hbar^2f_x$. Thus an answer is $\sin\theta\cos\phi$. Its squared [norm](../../../../../norm.md) on the sphere is

$$
\int_0^{2\pi}\cos^2\phi\,d\phi\int_0^\pi\sin^3\theta\,d\theta=\pi\frac43=\frac{4\pi}3,
$$

so the normalized [quantum state](../../../../../quantum-state.md) is

$$
\boxed{\psi_x(\theta,\phi)=\sqrt{\frac3{4\pi}}\sin\theta\cos\phi,\qquad L^2\psi_x=2\hbar^2\psi_x,\qquad L_1\psi_x=0.}
$$

The supplied starting state gives an alternative derivation with a changed [quantization axis](../../../../../quantization-axis.md). Put $g=\cos\theta+i\sin\theta\sin\phi$ and $K_+=L_2+iL_3$. The [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) give $[L_1,K_+]=\hbar K_+$ and $[L^2,K_+]=0$, so $K_+$ raises the $L_1$ projection from $-\hbar$ to zero. Direct differentiation gives

$$
L_2g=i\hbar\sin\theta\cos\phi,\qquad L_3g=\hbar\sin\theta\cos\phi,\qquad K_+g=2i\hbar\sin\theta\cos\phi,
$$

which is nonzero and proportional to the same $\psi_x$. This also connects the construction directly to the given state.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
