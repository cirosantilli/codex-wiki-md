<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $S_Nf(t)=\sum_{|n|\leq N}\widehat f(n)e^{int}$ for the symmetric [Fourier partial sum](../../../../../fourier-partial-sum.md), with normalized [Fourier coefficients](../../../../../fourier-coefficient.md) on $\mathbb T=\mathbb R/(2\pi\mathbb Z)$. We will prove the stronger conclusion

$$
\boxed{\limsup_{N\to\infty}|S_Nf(t)|=\infty\quad\text{for every }t\in E.}
$$

If $E$ is empty, take $f=0$. Otherwise the proof of the [Kahane-Katznelson divergence theorem](../../../../../kahane-katznelson-divergence-theorem.md) has three steps: a bounded [trigonometric polynomial](../../../../../trigonometric-polynomial.md) whose partial sum is large on short arcs, a finite-arc batching of an arbitrary null set, and a uniformly convergent sequence of separated frequency blocks. In particular, no assumption that $E$ is closed or compact is needed.

First consider a nonempty finite family of arcs with centers $\theta_\nu$, half-lengths $0<d_\nu\leq1$, and $D=\sum_\nu d_\nu$. On the closed unit disk define

$$
\Phi(z)=\sum_\nu\frac{d_\nu}{D}\frac{1+d_\nu}{1+d_\nu-ze^{-i\theta_\nu}}.
$$

Each summand has positive real part there, and $\Phi(0)=1$. Thus the principal [complex logarithm](../../../../../complex-logarithm.md) $A=\log\Phi$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a neighborhood of the closed disk, $A(0)=0$, and $|\operatorname{Im}A|<\pi/2$. To bound its real part on an arc, put $h=t-\theta_\nu$ with $|h|\leq d_\nu$ and $q=1+d_\nu-\cos h$. Then

$$
d_\nu\leq q\leq\tfrac32d_\nu,\qquad |\sin h|\leq d_\nu,\qquad \operatorname{Re}\frac{1+d_\nu}{1+d_\nu-e^{ih}}=\frac{(1+d_\nu)q}{q^2+\sin^2h}\geq\frac4{13d_\nu}>\frac1{4d_\nu}.
$$

After multiplication by the weight $d_\nu/D$, this contribution is at least $1/(4D)$; all the other contributions have positive real part. Throughout the arc union we therefore have

$$
\operatorname{Re}\Phi(e^{it})\geq\frac1{4D},\qquad \operatorname{Re}A(e^{it})=\log|\Phi(e^{it})|\geq\log\frac1{4D}.
$$

This is the [positive-real logarithmic amplifier for short arcs](../../../../../positive-real-logarithmic-amplifier-for-short-arcs.md). Since $A$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) beyond the closed unit disk, its [Taylor series](../../../../../taylor-series.md) converges uniformly there. Choose a polynomial $Q(z)=\sum_{\nu=1}^{d}a_\nu z^\nu$ with $\sup_{|z|\leq1}|Q(z)-A(z)|<1$. There is no constant term because $A(0)=0$. Set $C=\pi/2+1$ and

$$
B(t)=\operatorname{Im}Q(e^{it})=\frac{Q(e^{it})-\overline{Q(e^{it})}}{2i},\qquad P(t)=\frac{e^{iMt}}C B(t),
$$

where the integer $M>d$ may be chosen arbitrarily large. We have $\|P\|_\infty\leq1$, and its frequencies lie in $[M-d,M+d]$. At the cut $N=M$, the positive-frequency half of $Q$ is excluded and the negative-frequency half is included. Hence

$$
S_MP(t)=-\frac{e^{iMt}}{2iC}\overline{Q(e^{it})},\qquad |S_MP(t)|\geq\frac{\log(1/(4D))-1}{2C}
$$

on the arc union. In particular, for any $K>0$, a total half-length $D\leq\tfrac14e^{-1-2CK}$ gives $|S_MP|\geq K$ there. This proves the needed [compact-set Fourier amplification lemma](../../../../../compact-set-fourier-amplification-lemma.md), with the additional freedom to place its entire frequency block above any prescribed frequency.

Next we construct the [null-set limsup cover by finite arc families](../../../../../null-set-limsup-cover-by-finite-arc-families.md). Set

$$
a_j=2^{-j},\qquad K_j=2^j(j+2),\qquad D_j=\tfrac14e^{-1-2CK_j}\quad(j\geq1).
$$

Since $E$ has [Lebesgue measure](../../../../../lebesgue-measure.md) zero, for every row $\ell\geq1$ choose a countable arc cover $\{I_{\ell,m}:m\geq1\}$ of $E$ with positive half-lengths $d_{\ell,m}$ and $\sum_m d_{\ell,m}<2^{-\ell}D_1$. We can take closed arcs by slightly enlarging an open cover; their half-lengths are less than one. The whole two-index array has total half-length less than $D_1$. Absolute convergence of this sum lets us choose strictly increasing integers $N_j$ such that the sum outside the finite square $1\leq\ell,m\leq N_j$ is less than $D_{j+1}$. Put $N_0=0$ and let $\mathcal F_j$ contain those arcs for which

$$
N_{j-1}<\max(\ell,m)\leq N_j.
$$

Each family is finite. Its total half-length is less than $D_j$: for $j=1$ use the total sum, and for $j>1$ use the tail outside the preceding square. Moreover, every $t\in E$ belongs to arcs with unbounded row index, so belongs to the unions of infinitely many of the families $\mathcal F_j$. This batching is essential: a dense null set need not have a finite cover of small total length, whereas the infinitely-often finite covers above suffice.

Apply the amplification construction to $\mathcal F_j$ with height $K_j$, obtaining $P_j$ with $\|P_j\|_\infty\leq1$ and $|S_{M_j}P_j(t)|\geq K_j$ on that family's union. Choose the modulation integers successively so that the frequency intervals $[M_j-d_j,M_j+d_j]$ are positive and each lies strictly above the preceding one. Empty families may be represented by $P_j=0$ and an unused frequency interval. Define the [frequency-separated Fourier block series](../../../../../frequency-separated-fourier-block-series.md)

$$
f(t)=\sum_{j=1}^{\infty}a_jP_j(t).
$$

The bound $\sum_j a_j\|P_j\|_\infty\leq1$ gives absolute [uniform convergence](../../../../../uniform-convergence.md), so $f$ is continuous. Uniform convergence also justifies computing every [Fourier coefficient](../../../../../fourier-coefficient.md) term by term. At frequency $M_j$, all earlier blocks have been included in full and all later blocks are absent:

$$
S_{M_j}f(t)=\sum_{i<j}a_iP_i(t)+a_jS_{M_j}P_j(t).
$$

For $t$ in the union of $\mathcal F_j$, the reverse [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|S_{M_j}f(t)|\geq a_jK_j-\sum_{i<j}a_i\geq j+1.
$$

Every $t\in E$ lies in infinitely many such unions, and $M_j\to\infty$. Therefore the boxed unboundedness holds at every point of $E$, completing the proof for arbitrary null sets.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
