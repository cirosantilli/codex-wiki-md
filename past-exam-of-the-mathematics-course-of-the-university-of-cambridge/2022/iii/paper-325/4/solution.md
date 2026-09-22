<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Schmidt decomposition](../../../../../schmidt-decomposition.md) of an entangled pure two-qubit state has two nonzero terms. Absorb both complex phases into the local basis vectors and interchange the labels of the second qubit to obtain

$$
|\psi\rangle=c_0|\uparrow\rangle_1|\downarrow\rangle_2
+c_1|\downarrow\rangle_1|\uparrow\rangle_2,
\qquad
c_0,c_1>0,
\qquad
c_0^2+c_1^2=1.
$$

In this state the only nonzero same-axis two-qubit [Pauli correlators](../../../../../pauli-correlator.md) are

$$
\langle X\otimes X\rangle
=\langle Y\otimes Y\rangle=2c_0c_1,
\qquad
\langle Z\otimes Z\rangle=-1.
$$

All mixed-axis correlators vanish. Expanding $(\mathbf a\cdot\boldsymbol\sigma)\otimes(\mathbf b\cdot\boldsymbol\sigma)$ therefore gives

$$
\boxed{E(\mathbf a,\mathbf b)
=2c_0c_1(a_xb_x+a_yb_y)-a_zb_z}.
$$

For the four stated vectors this becomes

$$
E(\mathbf a,\mathbf b)=-\cos\beta,
\quad
E(\mathbf a,\mathbf b')=-\cos\beta',
\quad
E(\mathbf a',\mathbf b)=-2c_0c_1\sin\beta,
\quad
E(\mathbf a',\mathbf b')=-2c_0c_1\sin\beta'.
$$

It follows immediately that

$$
|E(\mathbf a,\mathbf b)-E(\mathbf a,\mathbf b')|
+|E(\mathbf a',\mathbf b)+E(\mathbf a',\mathbf b')|
=|\cos\beta-\cos\beta'|
+2c_0c_1|\sin\beta+\sin\beta'|.
$$

Every [separable quantum state](../../../../../separable-quantum-state.md) obeys the corresponding [CHSH inequality](../../../../../chsh-inequality.md) with upper bound two. Set $s=2c_0c_1>0$, choose $\beta'=\pi-\beta$, and take $\tan\beta=s$ with $0<\beta<\pi/2$. The displayed expression is then

$$
2(\cos\beta+s\sin\beta)=2\sqrt{1+s^2}>2.
$$

Thus every entangled pure two-qubit state has local measurement correlations that no separable state can reproduce, which is [Gisin's theorem](../../../../../gisin-s-theorem.md). In an ideal [Bose--Marletto--Vedral experiment](../../../../../bose-marletto-vedral-experiment.md), optimized local measurements can therefore witness any nonzero pure-state entanglement generated during the gravitational interaction. If gravity is the only interaction between the masses, such a violation shows that the mediator cannot be described by a purely classical local variable under the assumptions of the proposal; experimentally, control of [decoherence](../../../../../quantum-decoherence.md) and nongravitational forces is essential to that inference.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
