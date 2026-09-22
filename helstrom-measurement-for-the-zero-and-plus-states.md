# Helstrom measurement for the zero and plus states

↑ **Parent:** [Helstrom measurement for two pure states](helstrom-measurement-for-two-pure-states.md)

Suppose one [qubit](qubit.md) is prepared in either of the known [pure states](pure-state.md) $|0\rangle$ and $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$, with equal prior [probabilities](probability.md). Measuring in the [computational basis](computational-basis.md) seems natural, but a tilted [projective measurement](projective-measurement.md) gives better [quantum state discrimination](quantum-state-discrimination.md). The two [density operators](density-matrix.md) and their difference are

$$
\rho_0=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
\rho_+=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},\qquad
\Delta=\rho_0-\rho_+=\frac12\begin{pmatrix}1&-1\\-1&-1\end{pmatrix}
=\frac12(\sigma_z-\sigma_x).
$$

The [Pauli matrices](pauli-matrices.md) give $\Delta^2=I/2$, and the [eigenvalues](eigenvalue.md) of $\Delta$ are $\lambda_\pm=\pm1/\sqrt2$. Their absolute sum gives [trace distance](trace-distance.md) $D=1/\sqrt2$, agreeing with [trace distance between qubit states](trace-distance-between-qubit-states.md).

The positive [spectral projector](spectral-projector.md) points along the unit [Bloch vector](bloch-vector.md) $\mathbf n=(-1,0,1)/\sqrt2$:

$$
P_+=\frac{I+\mathbf n\cdot\boldsymbol\sigma}{2}
=\frac12\left(I+\frac{\sigma_z-\sigma_x}{\sqrt2}\right),\qquad
P_-=I-P_+.
$$

The outcome labels $+$ and $-$ here refer to the sign of the [eigenvalue](eigenvalue.md) of $\Delta$; they do not denote a [Hadamard basis](hadamard-basis.md) measurement. Guess $|0\rangle$ after $P_+$ and $|+\rangle$ after $P_-$. This sign choice is the equal-prior [Helstrom measurement for two pure states](helstrom-measurement-for-two-pure-states.md), a case of the [Holevo–Helstrom theorem](holevo-helstrom-theorem.md). [Watrous, The Theory of Quantum Information, Theorem 3.4, equation (3.17)](https://cs.uwaterloo.ca/~watrous/TQI/TQI.3.pdf)

An explicit [orthonormal basis](orthonormal-basis.md) for this [projective measurement](projective-measurement.md) is

$$
|h_+\rangle=\cos(\pi/8)|0\rangle-\sin(\pi/8)|1\rangle,\qquad
|h_-\rangle=\sin(\pi/8)|0\rangle+\cos(\pi/8)|1\rangle,
$$

with $P_\pm=|h_\pm\rangle\langle h_\pm|$. Thus the real coefficient rotation angle is $\beta=-\pi/8$ relative to the [computational basis](computational-basis.md), while the [Bloch vector](bloch-vector.md) of $P_+$ is tilted by $\pi/4$ from the positive $z$ axis toward negative $x$. State-vector and [Bloch sphere](bloch-sphere.md) angles differ by a factor of two.

Write $a=(1+1/\sqrt2)/2$ and $b=(1-1/\sqrt2)/2$, so $a+b=1$. The [Born rule](born-rule.md) gives the conditional outcome [probabilities](probability.md)

$$
\begin{array}{c|cc}
\text{input}&P_+&P_-\\\hline
\rho_0&a&b\\
\rho_+&b&a
\end{array}
\qquad
a\simeq0.853553,\quad b\simeq0.146447.
$$

The event $P_+$ has [probability](probability.md) gap $a-b=1/\sqrt2=D$, attaining the [variational characterization of trace distance](variational-characterization-of-trace-distance.md). Both preparations are identified correctly with conditional [probability](probability.md) $a$, so

$$
P_{\mathrm{success}}^{\mathrm{opt}}=\frac{a+a}{2}
=\frac12\left(1+\frac1{\sqrt2}\right)\simeq0.853553.
$$

For comparison, a $Z$ [projective measurement](projective-measurement.md) in the [computational basis](computational-basis.md) has conditional outcome [probabilities](probability.md) $(1,0)$ on $\rho_0$ and $(1/2,1/2)$ on $\rho_+$. Guess zero on outcome zero and plus on outcome one. The average success is

$$
P_{\mathrm{success}}^{Z}=\frac12\left(1+\frac12\right)=\frac34,
$$

and the measured [total variation distance](total-variation-distance.md) is only $1/2$. The optimal tilted [projective measurement](projective-measurement.md) gains about $0.103553$ in absolute success [probability](probability.md) by balancing the two conditional error rates instead of identifying $|0\rangle$ perfectly at the expense of $|+\rangle$.

<a id="image-conditional-outcome-probabilities-and-equal-prior-success-for-z-and-optimal-helstrom-measurements-of-zero-versus-plus"></a>
![](helstrom-zero-plus-measurement.png)

**[Figure 6](#image-conditional-outcome-probabilities-and-equal-prior-success-for-z-and-optimal-helstrom-measurements-of-zero-versus-plus). Conditional outcome probabilities and equal-prior success for Z and optimal Helstrom measurements of zero versus plus**.

These are statistics for alternative measurements on independently prepared copies. Applying $Z$ first and then the tilted [projective measurement](projective-measurement.md) is a different experiment, because the first [measurement in quantum mechanics](quantum-measurement-split.md) changes the [density operator](density-matrix.md).

## ↑ Ancestors (6)

1. [Helstrom measurement for two pure states](helstrom-measurement-for-two-pure-states.md)
2. [Helstrom-Holevo bound](helstrom-holevo-bound.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/10d/a/solution.md)
- [Trace distance between qubit states](trace-distance-between-qubit-states.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
