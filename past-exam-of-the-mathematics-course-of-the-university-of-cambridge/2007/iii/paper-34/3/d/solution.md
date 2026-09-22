<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Holevo-Schumacher-Westmoreland theorem](../../../../../../holevo-schumacher-westmoreland-theorem.md) gives the classical coding formula

$$
C(\Phi)=\lim_{m\to\infty}\frac1m\chi^*(\Phi^{\otimes m}),\qquad\chi^*(\Lambda)=\sup_{\{p_i,\rho_i\}}\chi(\{p_i,\Lambda(\rho_i)\}).
$$

Its ensemble-coding statement makes every rate below a one-use output [Holevo quantity](../../../../../../holevo-quantity.md) achievable with product input encodings and collective output decoding. Under this product-input restriction, the capacity is

$$
C_{\mathrm{prod}}(\Phi)=\sup_{\{p_i,\rho_i\}}\chi(\{p_i,\Phi(\rho_i)\}).
$$

For any such input ensemble, rates below its output [Holevo quantity](../../../../../../holevo-quantity.md) are achievable with asymptotically vanishing decoding error. Maximization gives the [product-state classical capacity](../../../../../../holevo-capacity.md). The converse follows from the [Holevo bound](../../../../../../holevo-s-theorem.md), entropy bounds on product outputs, and [Fano's inequality](../../../../../../fano-s-inequality.md).

Define the [binary entropy](../../../../../../binary-entropy.md) $h_2(x)=-x\log_2x-(1-x)\log_2(1-x)$. For an input Bloch radius $r\leq1$, the output eigenvalues are $(1\pm(1-q)r)/2$. Its entropy is

$$
S(\Phi(\rho))=h_2\left(\frac{1+|1-q|r}{2}\right).
$$

On $[1/2,1]$, $h_2$ is decreasing, so this is minimized by pure inputs $r=1$. Throughout the completely positive interval $0\leq q\leq4/3$, the minimum equals $h_2(q/2)$, using symmetry $h_2(x)=h_2(1-x)$. The average output entropy is at most $1$, because it is a qubit. Hence every ensemble satisfies

$$
\chi(\{p_i,\Phi(\rho_i)\})\leq1-h_2(q/2).
$$

Two equally likely orthogonal pure inputs attain this bound: their average output is $I/2$, and each individual output has entropy $h_2(q/2)$. Therefore

$$
\boxed{C_{\mathrm{prod}}(\Phi)=1-h_2(q/2)=1-h_2(2p/3)\quad\text{bits per channel use}.}
$$

This gives the [Holevo capacity of a qubit depolarizing channel](../../../../../../holevo-capacity-of-a-qubit-depolarizing-channel.md) in the noise-weight convention used here.

For completeness, correlated classical code labels do not evade this upper bound. Each product input to $n$ uses has product output entropy at least $nh_2(q/2)$, whereas the average output entropy is at most $n$. Its [Holevo quantity](../../../../../../holevo-quantity.md) is consequently at most $n[1-h_2(q/2)]$. The [Holevo bound](../../../../../../holevo-s-theorem.md) and [Fano's inequality](../../../../../../fano-s-inequality.md) rule out a reliable rate larger than this value. Combined with HSW achievability, this proves the capacity under the stated product-input restriction. It also remains valid in the extended physical parameter range arising from the original $p$ assumption.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
