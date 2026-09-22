<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppress the common time factor $e^{i\omega t}$ and invert the stated [Fourier transform](../../../../../fourier-transform.md) with $(2\pi)^{-1}\int\Phi(k,y)e^{-ikx}dk$. Use [limiting absorption principle](../../../../../limiting-absorption-principle.md) $k_0\mapsto k_0-i0$, and choose $\gamma=\sqrt{k^2-k_0^2}$ with positive real part for the evanescent spectrum. For $|k|<k_0$ its outgoing continuation is $\gamma=+i\sqrt{k_0^2-k^2}$. The pole $-k_0$ lies above the inversion contour and $+k_0$ below it. These prescriptions fix both radiation and pole signs.

The even interior scattered transform solves $\Phi_{yy}-\gamma^2\Phi=0$, so it is $A(k)\cosh(\gamma y)$. The exterior transform is $B(k)e^{-\gamma(|y|-b)}$. Let $D^-(k)$ be the transform of their common upward normal derivative on $y=b$. On $x>0$ the rigid plates set both derivatives to zero; on $x<0$ continuity requires them to agree. Hence this derivative is supported on the negative half-line and is analytic below the transform contour. It follows that

$$
A=\frac{D^-}{\gamma\sinh(\gamma b)},\qquad B=-\frac{D^-}{\gamma}.
$$

The difference between exterior and interior scattered traces on $y=b$ is $-D^-/L$, where $L=\gamma\sinh(\gamma b)e^{-\gamma b}$. At the open negative half-line the total traces must match, so this difference equals the incident wave $e^{ik_0x}$. Its negative-half transform is $-i/(k+k_0)$. The positive-half trace difference has an unknown upper-half-plane transform $C^+$, giving the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md)

$$
-\frac{D^-}{L}=C^+-\frac{i}{k+k_0}.
$$

Factor $L=L^+L^-$, divide by $L^-$, and subtract the forcing pole using $C_0=L^+(-k_0)$:

$$
\frac{D^-}{L^-}-\frac{iC_0}{k+k_0}
=-L^+C^++i\frac{L^+(k)-C_0}{k+k_0}.
$$

The left side is analytic below and the right side above; the pole in the last quotient is removable. Analytic continuation makes their common value entire. The finite-energy edge condition and algebraic factor growth make this entire remainder vanish: the allowed normal-[velocity](../../../../../velocity.md) edge singularity is at most inverse-square-root, so its half-line transform is $O(|k|^{-1/2})$, while $L^\pm=O(|k|^{1/2})$. The same edge condition excludes a growing polynomial remainder. This [pole subtraction in a Wiener-Hopf equation](../../../../../pole-subtraction-in-a-wiener-hopf-equation.md) yields

$$
\boxed{D^-=\frac{iC_0L^-(k)}{k+k_0},\qquad
\Phi_{\rm sc}^{\rm in}=\frac{iC_0L^-(k)\cosh(\gamma y)}{\gamma\sinh(\gamma b)(k+k_0)}.}
$$

The corresponding exterior result for the [Wiener-Hopf solution for an open parallel-plate waveguide](../../../../../wiener-hopf-solution-for-an-open-parallel-plate-waveguide.md) is

$$
\boxed{\Phi_{\rm sc}^{\rm out}=-\frac{iC_0L^-(k)}{\gamma(k+k_0)}e^{-\gamma(|y|-b)}
=-\frac{iC_0\sinh(\gamma b)}{L^+(k)(k+k_0)}e^{-\gamma|y|}.}
$$

Both forms are useful: the first makes the common normal derivative transparent, and the second removes the apparent factor singularity at a grazing saddle.

The final unheaded request has a sign error in its printed exponent. To see this from the derived solution rather than an outgoing-decay assertion alone, simplify the interior transform to

$$
\Phi_{\rm sc}^{\rm in}=\frac{iC_0e^{-\gamma b}\cosh(\gamma y)}{L^+(k)(k+k_0)}.
$$

Near $k=-k_0$, $C_0/L^+(k)=1+O(k+k_0)$ and $e^{-\gamma b}\cosh(\gamma y)=1-b\gamma+O(\gamma^2)$ for fixed $|y|<b$. Thus

$$
\Phi_{\rm sc}^{\rm in}=\frac{i}{k+k_0}-\frac{ib\gamma}{k+k_0}+O(1).
$$

For $x<0$, inversion of the first term gives $-e^{ik_0x}$, cancelling the continued incident potential. The remaining branch-point term uses $\gamma\sim i\sqrt{2k_0}\,(k+k_0)^{1/2}$ on the specified contour, so it is $b\sqrt{2k_0}(k+k_0)^{-1/2}$. Its inverse transform at $x=-r$ is proportional to $e^{-ik_0r+i\pi/4}/\sqrt{\pi r}$. Therefore the [upstream decay of an open parallel-plate waveguide](../../../../../upstream-decay-of-an-open-parallel-plate-waveguide.md) is

$$
\boxed{\phi_{\rm tot}(x,y)\sim b\sqrt{\frac{2k_0}{\pi(-x)}}\,e^{ik_0x+i\pi/4},\qquad x\to-\infty,\quad |y|<b.}
$$

The [amplitude](../../../../../wave-amplitude.md) decays as $(-x)^{-1/2}$, not $(-x)^{1/2}$. The positive exponent is present in the original PDF, so it cannot be proved under the stated outgoing problem. The incident pole cancellation and the explicit branch expansion give the corrected conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
