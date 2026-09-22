<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Substitution of $w_i=f_i(y)e^{i(kx-\omega t)}$ gives

$$
\boxed{f_i''+\left(\frac{\omega^2}{c_{si}^2}-k^2\right)f_i=0.}
$$

The oscillatory seam solution requires $m^2=\omega^2/c_{s1}^2-k^2$, giving

$$
\boxed{\omega^2=c_{s1}^2(k^2+m^2),\qquad
c_L=\frac\omega{|k|}=c_{s1}\sqrt{1+m^2/k^2}.}
$$

For an exponentially decaying exterior, $f_2''=\ell^2f_2$ with $\ell>0$, so the same differential equation instead requires

$$
\boxed{\ell^2=k^2-\omega^2/c_{s2}^2,\qquad
\omega^2=c_{s2}^2(k^2-\ell^2).}
$$

The printed exterior plus sign is inconsistent with its decaying ansatz and must be a sign error. The guided mode has $c_{s1}<c_L<c_{s2}$, so a slower shear-wave seam than its cladding is necessary.

For an even seam mode $f_1=A\cos(my)$, upper-interface [displacement](../../../../displacement.md) and [traction](../../../../traction.md) continuity give

$$
A\cos(mh)=A_2e^{-\ell h},\qquad
-\mu_1Am\sin(mh)=-\mu_2\ell A_2e^{-\ell h}.
$$

The lower interface gives the same equations when $B_2=A_2$. Eliminating the amplitudes yields

$$
\boxed{\mu_1m\tan(mh)=\mu_2\ell.}
$$

For an odd seam mode $f_1=B\sin(my)$, the equations are

$$
B\sin(mh)=A_2e^{-\ell h},\qquad
\mu_1Bm\cos(mh)=-\mu_2\ell A_2e^{-\ell h}.
$$

With $B_2=-A_2$ the lower condition agrees, and elimination gives

$$
\boxed{\mu_1m\cot(mh)=-\mu_2\ell.}
$$

These interface conditions together with the two corrected dispersion identities determine the guided-wave branches.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
