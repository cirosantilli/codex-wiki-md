<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce $t_0=t$, $T_1=\epsilon t$, $T=\epsilon^2t$ and write $x=x_0+\epsilon x_1+\cdots$. The [method of multiple scales](../../../../../../method-of-multiple-scales.md) gives $x_0=A(T_1,T)e^{it_0}+\overline A e^{-it_0}$. At order $\epsilon$, the resonant forcing is $-2\partial_{t_0}\partial_{T_1}x_0$, because multiplication by $\cos t_0$ generates only a constant and second harmonics. The [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) therefore gives $A_{T_1}=0$. A nonresonant particular correction is

$$
x_1=\frac A6e^{2it_0}+\frac{\overline A}6e^{-2it_0}-\frac{A+\overline A}{2}.
$$

At order $\epsilon^2$, the forcing is $-2\partial_{t_0}\partial_Tx_0-fx_0-\cos t_0x_1$. Its $e^{it_0}$ coefficient is $-2iA_T+(1/6-f)A+\overline A/4$. Removing this [secular term](../../../../../../secular-term.md) gives

$$
2iA_T=(1/6-f)A+\overline A/4.
$$

Put $A=(a-ib)/2$, so $x_0=a(T)\cos t+b(T)\sin t$. The [slow amplitudes for the second Mathieu instability tongue](../../../../../../slow-amplitudes-for-the-second-mathieu-instability-tongue.md) satisfy

$$
a_T=\frac{f+1/12}{2}b,\qquad b_T=\frac{5/12-f}{2}a,\qquad a(0)=1,\ b(0)=0.
$$

The initial conditions here are at leading order; a homogeneous $O(\epsilon)$ correction makes the original data exact without changing $x_0$. For example its initial cosine coefficient is $2/3$ in the chosen $x_1$ gauge. The slow squared growth rate is $(f+1/12)(5/12-f)/4$. Thus the robust leading stable ranges are

$$
\boxed{f<-1/12\quad\text{or}\quad f>5/12.}
$$

Set $\nu=\tfrac12\sqrt{(f+1/12)(f-5/12)}$ in those ranges. The required explicit leading solution is

$$
\boxed{x(t;\epsilon)=\cos(\nu\epsilon^2t)\cos t+
\frac{5/12-f}{2\nu}\sin(\nu\epsilon^2t)\sin t+O(\epsilon).}
$$

The remainder is uniform for $0\le\epsilon^2t\le C$, with fixed $C$ and fixed $f$ away from a changing instability edge. Inside $-1/12<f<5/12$, put $\sigma=\tfrac12\sqrt{(f+1/12)(5/12-f)}$; replace the slow cosine and $\sin(\nu T)/\nu$ by $\cosh(\sigma T)$ and $\sinh(\sigma T)/\sigma$. The initial data excite this growing solution, so the leading solution is unstable.

At the leading endpoints the slow matrix is degenerate. Its continuous limits give $x_0=\cos t+(T/4)\sin t$ at $f=-1/12$, and $x_0=\cos t$ for these particular initial data at $f=5/12$; generic initial phases at the latter endpoint have slow algebraic growth. These are leading, not exact, instability edges. To specify the exact small-$\epsilon$ endpoint status, put $t=2s$, so the [Mathieu equation](../../../../../../mathieu-equation.md) has characteristic parameter $a_M=4+4f\epsilon^2$ and coupling $q_M=-2\epsilon$. In the orthonormal cosine basis $1,\cos2s,\cos4s,\cos6s$, the matrix has diagonal $0,4,16,36$ and adjacent couplings $\sqrt2q_M,q_M,q_M$; in the sine basis $\sin2s,\sin4s,\sin6s$, the diagonal is $4,16,36$ and adjacent couplings are $q_M,q_M$. Expanding the roots near $4$ of their determinants yields

$$
a_2=4+\frac5{12}q_M^2-\frac{763}{13824}q_M^4+O(q_M^6),\quad
b_2=4-\frac1{12}q_M^2+\frac5{13824}q_M^4+O(q_M^6).
$$

These truncations determine the displayed orders because reaching the next omitted mode and returning requires at least six coupling steps. The [fourth-order edges of the second Mathieu instability tongue](../../../../../../fourth-order-edges-of-the-second-mathieu-instability-tongue.md) are therefore

$$
f_-=-\frac1{12}+\frac5{3456}\epsilon^2+O(\epsilon^4),\qquad
f_+=\frac5{12}-\frac{763}{3456}\epsilon^2+O(\epsilon^4).
$$

[Floquet theory](../../../../../../floquet-theory.md) gives the unstable gap $f_-<f<f_+$ near this resonance. In particular, both fixed values $-1/12$ and $5/12$ lie outside the exact gap for sufficiently small nonzero $\epsilon$. Their fixed-$\epsilon$ solutions are bounded, although the leading slow matrix alone does not show this and the amplification bound is not uniform as $\epsilon\to0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
