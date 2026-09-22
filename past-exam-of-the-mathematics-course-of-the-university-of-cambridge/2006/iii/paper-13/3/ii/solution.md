<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The positive-power length assertion is an asymptotic one: it requires $N$ sufficiently large in terms of the density. Read literally for every $N$, it fails when $N=2$, $\delta=1/2$ and $A=\{1\}$, whose triple [sumset](../../../../../../sumset.md) is a singleton. We prove the intended result with this necessary qualification and an explicit positive exponent.

Embed the interval into the [cyclic group](../../../../../../cyclic-group.md) $G=\mathbb Z/M\mathbb Z$ with $M=8N$, and set $u=1_A$, $\alpha=|A|/M\geq\delta/8$. Since all integer triple sums lie in $[3,3N]$, this embedding introduces no collisions between distinct sums. Use normalized [Fourier coefficients on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) and [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md), and put

$$
F=u*u*u,\qquad F(t)=\frac1{M^2}\#\{(a,b,c)\in A^3:a+b+c=t\pmod M\}.
$$

The function $F$ is nonnegative and has mean $\alpha^3$, so some $t_0$ satisfies $F(t_0)\geq\alpha^3$. We show that a whole translated [Bohr set](../../../../../../bohr-set.md) is contained in its positive support, hence in the triple [sumset](../../../../../../sumset.md).

Put $\theta=\alpha^2/8$, $\rho=\alpha/4$, and define the [large spectrum](../../../../../../large-spectrum.md)

$$
\Gamma=\{r\in G:|\widehat u(r)|\geq\theta\},\qquad B=\{b\in G:|e^{2\pi irb/M}-1|\leq\rho\text{ for all }r\in\Gamma\}.
$$

The [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) gives $\sum_r|\widehat u(r)|^2=\alpha$, so

$$
|\Gamma|\leq\frac\alpha{\theta^2}=64\alpha^{-3}.
$$

Also $|\widehat u(r)|\leq\alpha$, and therefore $\sum_r|\widehat u(r)|^3\leq\alpha^2$. Using [Fourier inversion](../../../../../../fourier-inversion-theorem.md) and the [convolution theorem on a finite group](../../../../../../convolution-theorem-on-a-finite-group.md), for $b\in B$ we obtain

$$
\begin{aligned}
|F(t+b)-F(t)|&\leq\sum_r|\widehat u(r)|^3|e^{2\pi irb/M}-1|\\
&\leq\rho\sum_{r\in\Gamma}|\widehat u(r)|^3+2\sum_{r\notin\Gamma}|\widehat u(r)|^3\\
&\leq\rho\alpha^2+2\theta\sum_r|\widehat u(r)|^2=\frac{\alpha^3}{2}.
\end{aligned}
$$

Consequently $F(t_0+b)\geq\alpha^3/2>0$. This proves the [translated Bohr neighborhood in a triple sumset](../../../../../../translated-bohr-neighborhood-in-a-triple-sumset.md):

$$
t_0+B\subseteq A+A+A\pmod M.
$$

It remains to produce a long ordinary integer [arithmetic progression](../../../../../../arithmetic-progression.md) in this translate; we supply the simultaneous approximation and the lifting argument. Set

$$
D=\left\lceil64(8/\delta)^3\right\rceil,\qquad Q=\left\lfloor M^{1/(D+1)}\right\rfloor.
$$

Thus $d=|\Gamma|\leq D$. Partition the $d$-dimensional unit cube into $Q^d$ boxes of side $1/Q$. The $Q^d+1$ points

$$
\left(\frac{jr}{M}\pmod1\right)_{r\in\Gamma},\qquad 0\leq j\leq Q^d,
$$

contain two in the same box by the [pigeonhole principle](../../../../../../pigeonhole-principle.md). Their index difference gives an integer $q$ with $1\leq q\leq Q^d<M$ and

$$
\left\|\frac{qr}{M}\right\|_{\mathbb R/\mathbb Z}\leq\frac1Q\qquad(r\in\Gamma).
$$

In particular $|e^{2\pi irq/M}-1|\leq2\pi/Q$. The identity $z^j-1=(z-1)(1+\cdots+z^{j-1})$ on the unit circle now shows that

$$
0,q,2q,\ldots,(L-1)q\in B,\qquad L=\left\lfloor\frac{\rho Q}{2\pi}\right\rfloor+1.
$$

All residues $t_0+jq$ therefore lie in the triple [sumset](../../../../../../sumset.md). Let $s_j\in[3,3N]$ be their actual integer representatives. Their successive differences are congruent to $q$ modulo $M$, and each lies in $[-(3N-3),3N-3]$, which is contained in $(-M/2,M/2)$. There is at most one integer in this interval in any specified residue class, so every difference $s_{j+1}-s_j$ is the same integer. It is nonzero because $0<q<M$. Thus the $s_j$ form an ordinary integer [arithmetic progression](../../../../../../arithmetic-progression.md) of distinct elements, even though $M$ is composite. Reversing it if necessary makes the common difference positive.

For sufficiently large $N$, we have $Q\geq\tfrac12M^{1/(D+1)}$ and $\rho\geq\delta/32$, whence

$$
L\geq\frac{\rho Q}{2\pi}\geq\frac\delta{128\pi}N^{1/(D+1)}.
$$

Absorb this fixed prefactor by decreasing the exponent: with

$$
\boxed{r_\delta=\frac1{2(D+1)}>0,\qquad D=\left\lceil32768\delta^{-3}\right\rceil,}
$$

the last lower bound is at least $N^{r_\delta}$ once $N$ is sufficiently large in terms of $\delta$. This proves **a polynomial-length progression in $A+A+A$** by the [polynomial-length progression in a dense triple sumset](../../../../../../polynomial-length-progression-in-a-dense-triple-sumset.md) argument, without replacing the triple [sumset](../../../../../../sumset.md) by a fourfold difference set.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
