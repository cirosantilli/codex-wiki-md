<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

First prove the [convolution theorem](../../../../convolution-theorem.md) with the stated negative-exponential [Fourier transform](../../../../fourier-transform-split.md). Assuming absolute integrability sufficient for [Fubini's theorem](../../../../fubini-s-theorem.md), change variables $u=t-s$:

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikt}f(s)g(t-s)\,ds\,dt\\
&=\int_{\mathbb R}f(s)e^{-iks}ds\int_{\mathbb R}g(u)e^{-iku}du
=\widetilde f(k)\widetilde g(k).
\end{aligned}
$$

For the differential equation, [integration by parts](../../../../integration-by-parts.md) gives

$$
\widetilde {y'}=[e^{-ikt}y]_{-\infty}^\infty+ik\widetilde y=ik\widetilde y,
\qquad \widetilde {y''}=ik\widetilde {y'}=-k^2\widetilde y.
$$

The boundary terms vanish by the assumed decay of $y,y'$. As with the convolution step, the transforms can first be justified for integrable functions and derivatives; the resulting kernel gives the desired decaying response. Thus

$$
\boxed{\widetilde y(k)=\frac{\widetilde f(k)}{(a+ik)(b+ik)}=\widetilde f(k)\widetilde G(k).}
$$

The [convolution theorem](../../../../convolution-theorem.md) and [Fourier inversion theorem](../../../../fourier-inversion-theorem.md) imply $y=f*G$.

For the inverse transform of $\widetilde G$, use

$$
\widetilde G(k)=\frac1{a-b}\left(\frac1{b+ik}-\frac1{a+ik}\right).
$$

The [poles](../../../../pole.md) are at $ib,ia$. For $t>0$, close the inverse-transform contour above; the residues of $e^{ikt}\widetilde G(k)$ there are $-ie^{-bt}/(a-b)$ and $ie^{-at}/(a-b)$. The inverse-transform factor $1/(2\pi)$ makes the answer $i$ times their sum. For $t<0$, close below, enclosing no poles. The large arcs vanish: the complete rational factor is $O(|k|^{-2})$ and the exponential is bounded on the appropriate semicircle. Therefore the [causal Green function of an overdamped oscillator](../../../../causal-green-function-of-an-overdamped-oscillator.md) is

$$
\boxed{G(t)=\begin{cases}0,&t<0,\\(e^{-bt}-e^{-at})/(a-b),&t\geq0.\end{cases}}
$$

It is continuous, with $G(0)=0$ and $G'(0^+)=1$, so $(D_t+a)(D_t+b)G=\delta(t)$. The response can also be written $y(t)=\int_{-\infty}^tG(t-s)f(s)ds$.

For the bilateral exponential forcing, split the real [integral](../../../../integral-split.md) at zero:

$$
\widetilde f(k)=\int_{-\infty}^0e^{(1-ik)t}dt+\int_0^\infty e^{-(1+ik)t}dt
=\frac1{1-ik}+\frac1{1+ik}=\boxed{\frac2{1+k^2}}.
$$

Consequently

$$
\boxed{\widetilde y(k)=\frac2{(1+k^2)(a+ik)(b+ik)}.}
$$

For negative time the lower half-plane contains only $k=-i$. The [residue](../../../../residue.md) of $e^{ikt}\widetilde y$ there is $ie^t/[(a+1)(b+1)]$. Clockwise closure makes the inverse transform $-i$ times that residue. For positive time the three upper [residues](../../../../residue.md), at $i,ia,ib$ respectively, are

$$
-\frac{ie^{-t}}{(a-1)(b-1)},\qquad
-\frac{2ie^{-at}}{(a^2-1)(a-b)},\qquad
\frac{2ie^{-bt}}{(b^2-1)(a-b)}.
$$

Multiplication of their sum by $i$ gives the [bilateral exponential forcing of an overdamped oscillator](../../../../bilateral-exponential-forcing-of-an-overdamped-oscillator.md):

$$
\boxed{y(t)=\begin{cases}
\dfrac{e^t}{(a+1)(b+1)},&t\leq0,\\
\dfrac{e^{-t}}{(a-1)(b-1)}+\dfrac2{a-b}\left(\dfrac{e^{-at}}{a^2-1}-\dfrac{e^{-bt}}{b^2-1}\right),&t\geq0.
\end{cases}}
$$

Both expressions have $y(0)=y'(0)=1/[(a+1)(b+1)]$. This verifies the matching that prevents an extra [Dirac delta function](../../../../dirac-delta-function.md) at zero. Direct substitution gives the forcing on either side, and all terms decay at their corresponding infinities. A causal [Green function](../../../../green-s-function-split.md) does not imply zero response before $t=0$ when the forcing has already been acting at negative times. The assumptions $a,b\ne1$ avoid repeated poles; their limiting cases would contain polynomial times exponential terms.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
