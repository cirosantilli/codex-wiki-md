<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $x=r\cos\theta$, $y=r\sin\theta$, and $s=|\sin\theta|$. From the exterior transform, the inverse integral has the [amplitude](../../../../../../wave-amplitude.md)

$$
f(k)=-\frac{iC_0\sinh(\gamma(k)b)}{2\pi L^+(k)(k+k_0)}
$$

multiplying $e^{-ikr\cos\theta-\gamma rs}$. Apply the supplied [method of steepest descent](../../../../../../method-of-steepest-descent.md) formula at $k_s=k_0\cos\theta$. On the outgoing sheet, $\gamma(k_s)=ik_0s$, so $-i\sinh(ik_0bs)=\sin(k_0bs)$. The far-field scattered potential is

$$
\boxed{\phi_{\rm sc}^{\rm out}(r,\theta)\sim
C_0\sqrt{\frac{k_0}{2\pi r}}\,
\frac{s\sin(k_0bs)}{L^+(k_0\cos\theta)(k_0\cos\theta+k_0)}
\,e^{-ik_0r+i\pi/4}.}
$$

Restore $e^{i\omega t}$ for the physical time-harmonic potential. This is cylindrical outgoing spreading, with angular directivity determined by the kernel factor and aperture. The ordinary saddle formula applies for a fixed non-grazing direction, away from a coalescing pole or branch point. Its finite upstream angular limit is consistent with the separate branch-point calculation in the root solution; at grazing directions that separate calculation supplies the appropriate justification.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
