<h1 id="4/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Alice verifies each submitted [qubit](../../../../../qubit.md) in her recorded secret basis and checks its bit against the revealed number. For a forger who chooses X or Z at random and prepares the corresponding known-bit [eigenstate](../../../../../eigenstate.md), each bit passes with [probability](../../../../../probability.md) $3/4$. With independent basis choices,

$$
\boxed{P_{\rm detect}^{\rm random}=1-\left(\frac34\right)^{24}
=0.9989966\ldots.}
$$

**The detection [probability](../../../../../probability.md) depends on Daisy's preparation strategy.** The question does not restrict her to legitimate X/Z [eigenstates](../../../../../eigenstate.md). Once the bit is known, for bit zero the averaged acceptance operator is

$$
A_0=\frac12\left(|0\rangle\langle0|+|+\rangle\langle+|\right)
=\frac I2+\frac{X+Z}{4}.
$$

For bit one it is $A_1=I-A_0$. Both have largest [eigenvalue](../../../../../eigenvalue.md) $p_{\rm opt}=(1+1/\sqrt2)/2$. Preparing the corresponding [eigenstate](../../../../../eigenstate.md), a [Bloch-vector](../../../../../bloch-vector.md) bisector of the two candidate encodings, achieves this value; for bit zero it is $\cos(\pi/8)|0\rangle+\sin(\pi/8)|1\rangle$.

The acceptance operator for the whole known check number is $\bigotimes_jA_{b_j}$, whose largest [eigenvalue](../../../../../eigenvalue.md) is $p_{\rm opt}^{24}$, so [entangled](../../../../../entangled-state.md) preparation cannot improve this no-original-note optimum. Therefore unrestricted preparation instead gives

$$
\boxed{P_{\rm detect}^{\rm optimal}=1-\left(\frac{1+1/\sqrt2}{2}\right)^{24}
=0.9776367\ldots.}
$$

The random-basis value is the elementary protocol calculation; the second value states the best forging strategy allowed by arbitrary state preparation and no access to the original quantum note.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [4](../../../4.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
