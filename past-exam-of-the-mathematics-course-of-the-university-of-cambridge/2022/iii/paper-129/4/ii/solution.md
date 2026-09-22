<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write

$$
\Lambda_4(f_1,f_2,f_3,f_4)
=\mathbb E_{x,d}f_1(x)f_2(x+d)f_3(x+2d)f_4(x+3d).
$$

Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) first in the variable carrying $f_1$ and then in the variable carrying $f_2$. After the invertible linear changes of variables permitted by $2,3\nmid|G|$, apply the assumed three-function $U^2$ estimate to the resulting multiplicative derivatives. The standard calculation gives

$$
|\Lambda_4|^8
\leq\|f_1\|_2^8\|f_2\|_2^8
\left(\mathbb E_h\|\partial_hf_3\|_{U^2}^4\right)
\left(\mathbb E_h\|\partial_hf_4\|_{U^2}^4\right).
$$

By the [Derivative identity for the Gowers U3 norm](../../../../../../derivative-identity-for-the-gowers-u3-norm.md), the last two factors are $\|f_3\|_{U^3}^8$ and $\|f_4\|_{U^3}^8$. Taking eighth roots proves

$$
|\Lambda_4(f_1,f_2,f_3,f_4)|
\leq\|f_1\|_2\|f_2\|_2\|f_3\|_{U^3}\|f_4\|_{U^3}.
$$

If $A\subseteq G$ has density $\alpha$, write $1_A=\alpha+f$. Expanding $\Lambda_4(1_A,1_A,1_A,1_A)$, the constant term is $\alpha^4$, and the displayed inequality bounds every nonconstant term after translation of one factor by a $U^3$ norm of the balanced function $f$. Thus sufficiently small $\|1_A-\alpha\|_{U^3}$ makes the normalized number of four-term [arithmetic progressions](../../../../../../arithmetic-progression.md) close to $\alpha^4$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
