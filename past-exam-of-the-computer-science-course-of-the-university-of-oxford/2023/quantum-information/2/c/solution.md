<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [three-way qutrit sign-flip discrimination](../../../../../three-way-qutrit-sign-flip-discrimination.md). Prepare the [qutrit](../../../../../qutrit.md) in the [uniform superposition state](../../../../../uniform-superposition-state.md)

$$
|s\rangle=\frac{|0\rangle+|1\rangle+|2\rangle}{\sqrt3}.
$$

For an unknown label $j\in\{0,1,2\}$, the supplied [unitary operator](../../../../../unitary-operator.md) is $U_j=I-2|j\rangle\langle j|$. Apply it once and then apply the known [inversion about the mean](../../../../../inversion-about-the-mean.md)

$$
D=2|s\rangle\langle s|-I
=\frac13\begin{pmatrix}-1&2&2\\2&-1&2\\2&2&-1\end{pmatrix}.
$$

Since $D^\dagger=D$ and $D^2=I$, this is an allowed [unitary transformation](../../../../../unitary-operator.md). Using $\langle s|j\rangle=1/\sqrt3$ gives

$$
DU_j|s\rangle
=D\left(|s\rangle-\frac2{\sqrt3}|j\rangle\right)
=-\frac13|s\rangle+\frac2{\sqrt3}|j\rangle
=\frac{5|j\rangle-\sum_{k\ne j}|k\rangle}{3\sqrt3}.
$$

Perform a [computational-basis measurement](../../../../../quantum-measurement-in-the-computational-basis.md) and guess that its outcome is the unknown label. The [Born rule](../../../../../born-rule.md) gives

$$
\boxed{\Pr(\text{correct}\mid U_j)=\left|\frac5{3\sqrt3}\right|^2=\frac{25}{27}.}
$$

Each incorrect outcome has [probability](../../../../../probability.md) $1/27$, verifying normalization. The success [probability](../../../../../probability.md) is $25/27$ separately for every label, so no assumption about their prior [probabilities](../../../../../probability.md) is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
