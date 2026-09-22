<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The final printed direction is reversed under the [majorization](../../../../../../majorization.md) convention stated in the same part. A completely depolarizing [unital quantum channel](../../../../../../unital-quantum-channel.md) sends a pure qubit state to $I/2$, giving spectra $r=(1,0)$ and $s=(1/2,1/2)$. The proposed $r\prec s$ fails already at the first partial sum, since $1>1/2$. The valid conclusion is

$$
\boxed{s\prec r.}
$$

Here is its general proof. Choose eigenbases $\rho=\sum_i r_i|u_i\rangle\langle u_i|$ and $\sigma=\sum_j s_j|v_j\rangle\langle v_j|$, and define the [eigenvalue mixing matrix of a unital quantum channel](../../../../../../eigenvalue-mixing-matrix-of-a-unital-quantum-channel.md)

$$
A_{ji}=\langle v_j|\Lambda(|u_i\rangle\langle u_i|)|v_j\rangle.
$$

Its entries are nonnegative by positivity. Trace preservation gives $\sum_jA_{ji}=1$ for every column. Unitality gives $\sum_iA_{ji}=\langle v_j|\Lambda(I)|v_j\rangle=1$ for every row. Thus $A$ is a [doubly stochastic matrix](../../../../../../doubly-stochastic-matrix.md), and linearity gives

$$
s_j=\sum_iA_{ji}r_i,\qquad s=Ar.
$$

The supplied doubly stochastic characterization of [majorization](../../../../../../majorization.md) then yields $s\prec r$, completing the intended corrected result. This proves [spectral majorization under a unital quantum channel](../../../../../../spectral-majorization-under-a-unital-quantum-channel.md). A [unital quantum channel](../../../../../../unital-quantum-channel.md) can make a spectrum more uniform; it cannot generally make the output spectrum majorize the input. The counterexample resolves the false printed assertion rather than treating the reversed inequality as a convention change.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
