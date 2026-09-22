<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [method of multiple scales](../../../../../../method-of-multiple-scales.md) with independent fast time $t$ and [slow time](../../../../../../slow-time.md) $T=\epsilon^2t$. A preliminary [slow time](../../../../../../slow-time.md) $\epsilon t$ produces no resonant forcing at first order, so its leading amplitudes are constant; the first nontrivial modulation is at $T$. Write $x=x_0+\epsilon x_1+\cdots$, with

$$
x_0=A(T)\cos t+B(T)\sin t.
$$

At order $\epsilon$, the [inhomogeneous linear differential equation](../../../../../../inhomogeneous-linear-differential-equation.md) is $(\partial_t^2+1)x_1=-\cos t\,x_0$. Absorbing its homogeneous part into the amplitudes gives

$$
x_1=-\frac A2+\frac A6\cos2t+\frac B6\sin2t.
$$

At order $\epsilon^2$, the forcing is $-2\partial_t\partial_Tx_0-kx_0-\cos t\,x_1$. Its resonant [Fourier series](../../../../../../fourier-series-split.md) coefficients are

$$
\left[-2B_T+\left(\frac5{12}-k\right)A\right]\cos t+
\left[2A_T-\left(k+\frac1{12}\right)B\right]\sin t.
$$

The [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) sets both coefficients to zero, giving the [amplitude equations](../../../../../../amplitude-equation.md). Define

$$
a=\frac{k+1/12}{2},\qquad b=\frac{5/12-k}{2},\qquad
M=\begin{pmatrix}0&a\\b&0\end{pmatrix}.
$$

For bounded [initial conditions](../../../../../../initial-condition.md) $x(0)=x_*$, $\dot x(0)=v_*$, the requested leading approximation is

$$
\boxed{x(t)=A(\epsilon^2t)\cos t+B(\epsilon^2t)\sin t+O(\epsilon),\qquad
\begin{pmatrix}A(T)\\B(T)\end{pmatrix}=e^{TM}\begin{pmatrix}x_*\\v_*\end{pmatrix},\qquad \beta=2.}
$$

This holds on bounded intervals of $T$, hence $t=O(\epsilon^{-2})$, with the constant in the error allowed to depend on the bounded $T$ interval. If desired, retain the displayed $\epsilon x_1$ and adjust $A(0),B(0)$ by $O(\epsilon)$ to match [initial conditions](../../../../../../initial-condition.md) at that order. No particular [initial conditions](../../../../../../initial-condition.md) were supplied.

Since $M^2=abI$, the [matrix exponential](../../../../../../matrix-exponential.md) is $I\cosh(\sigma T)+(M/\sigma)\sinh(\sigma T)$ when $\sigma^2=ab>0$. When $ab<0$, put $\omega=\sqrt{-ab}$ and replace this with $I\cos(\omega T)+(M/\omega)\sin(\omega T)$. At $ab=0$ it is $I+TM$. Thus the leading [second instability tongue of a weak Mathieu oscillator](../../../../../../second-instability-tongue-of-a-weak-mathieu-oscillator.md) has exponentially growing solutions for $-1/12<k<5/12$, and the leading modulation is bounded for every [initial condition](../../../../../../initial-condition.md) precisely when

$$
\boxed{k<-\frac1{12}\quad\text{or}\quad k>\frac5{12}.}
$$

At either displayed endpoint, $M$ is a nonzero [nilpotent operator](../../../../../../nilpotent-linear-map.md); some [initial conditions](../../../../../../initial-condition.md) give a [secular term](../../../../../../secular-term.md) proportional to $T$. This leading calculation alone must not be mistaken for an exact finite-$\epsilon$ stability decision at the endpoints.

For an exact small-$\epsilon$ interpretation, put $t=2s$. The standard [Mathieu equation](../../../../../../mathieu-equation.md) parameters are $a_{\rm M}=4+4k\epsilon^2$ and $q=-2\epsilon$. Its two relevant [Mathieu characteristic values](../../../../../../mathieu-characteristic-value.md) are obtained by projecting $-d^2/ds^2+2q\cos2s$ onto even and odd [Fourier series](../../../../../../fourier-series-split.md) modes. Near the unperturbed value $4$, the even modes $1,\cos2s,\cos4s,\cos6s$ have diagonal entries $0,4,16,36$ and adjacent couplings $\sqrt2q,q,q$ in an orthonormal basis; the odd modes $\sin2s,\sin4s,\sin6s$ have diagonal entries $4,16,36$ and couplings $q,q$. Substituting $4+c_2q^2+c_4q^4$ into their [characteristic polynomials](../../../../../../characteristic-polynomial.md) gives

$$
a_2(q)=4+\frac5{12}q^2-\frac{763}{13824}q^4+O(q^6),\qquad
b_2(q)=4-\frac1{12}q^2+\frac5{13824}q^4+O(q^6).
$$

Higher modes of the [Fourier series](../../../../../../fourier-series-split.md) first contribute at higher order. Therefore the [fourth-order edges of the second Mathieu instability tongue](../../../../../../fourth-order-edges-of-the-second-mathieu-instability-tongue.md) are

$$
k_-(\epsilon)=-\frac1{12}+\frac5{3456}\epsilon^2+O(\epsilon^4),\qquad
k_+(\epsilon)=\frac5{12}-\frac{763}{3456}\epsilon^2+O(\epsilon^4).
$$

[Floquet theory](../../../../../../floquet-theory.md) gives boundedness of every solution outside the closed gap, $k<k_-(\epsilon)$ or $k>k_+(\epsilon)$, in this fixed-$k=O(1)$ neighborhood. At the actual gap edges the second independent solution is generically unbounded. In particular, if $k$ is fixed exactly at $-1/12$ or $5/12$, it lies just outside the true gap and is stable for each sufficiently small positive $\epsilon$. The strict boxed criterion is the robust leading-order, uniformly separated criterion; the endpoints require this higher-order refinement, and their amplification bounds need not remain uniform as $\epsilon\to0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
