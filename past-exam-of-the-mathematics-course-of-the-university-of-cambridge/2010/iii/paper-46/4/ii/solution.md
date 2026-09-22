<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The ghost kinetic term as printed is $-\partial^\mu\bar c^a\partial_\mu c^a$. Integration by parts gives $\bar c^a\Box c^a$, so its Fourier-space quadratic kernel is $K_c^{ab}(p)=-p^2\delta^{ab}$. Completing the Grassmann square in the same generating functional gives

$$
Z_0[\bar\eta,\eta]=\exp[-i\bar\eta K_{c,F}^{-1}\eta].
$$

Keep the source order fixed, using a left derivative for $\bar\eta$ and a right derivative for $\eta$. Including the two insertion factors produces $\langle Tc\bar c\rangle=iK_{c,F}^{-1}$, just as in the [Gaussian generating functional for a Dirac field](../../../../../../gaussian-generating-functional-for-a-dirac-field.md). Therefore

$$
\boxed{\langle\Omega|T c^a(x)\bar c^b(y)|\Omega\rangle=\delta^{ab}\int\frac{d^4p}{(2\pi)^4}e^{-ip(x-y)}\frac{-i}{p^2+i0}.}
$$

The minus sign follows from the particular ghost Lagrangian in this paper. A convention with the opposite ghost kinetic sign has the opposite $c\bar c$ propagator; redefining the [Faddeev-Popov antighost field](../../../../../../faddeev-popov-antighost-field.md) changes its interaction and source signs at the same time. Mixing propagator and vertex conventions would give an erroneous loop sign. This is the [ghost propagator for a negative derivative kinetic term](../../../../../../ghost-propagator-for-a-negative-derivative-kinetic-term.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
