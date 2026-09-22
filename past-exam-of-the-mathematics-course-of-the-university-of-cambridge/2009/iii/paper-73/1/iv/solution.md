<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At a fixed location behind the advancing nose, the depth decreases after passage. A fall $-dh>0$ leaves the immobile fluid volume $s\phi(-dh)$ per unit length, so total local fluid storage changes by $\phi\,dh+s\phi(-dh)=\phi(1-s)\,dh$. The thinning-region equation is therefore

$$
\phi(1-s)h_t+uh_x=0.
$$

The inlet flux remains $uh(0,t)=Qe^{-t/\tau}$. Applying the [method of characteristics](../../../../../../method-of-characteristics.md) with thinning-wave speed $u/[\phi(1-s)]$ gives the [residual-trapping attenuation of a porous current](../../../../../../residual-trapping-attenuation-of-a-porous-current.md):

$$
\boxed{h(x,t)=h_0\exp\left[-\frac{t}{\tau}+\frac{\phi(1-s)x}{u\tau}\right],\qquad h_0=Q/u.}
$$

The nose advances into new pore space, which has no residual fluid yet, so its storage factor is still $\phi$ and its speed is still $u/\phi$. Consequently $X(t)=ut/\phi$ and the interior nose trace becomes $h_0e^{-st/\tau}$. Using the faster thinning-wave speed for the leading nose would incorrectly erase the attenuation caused by [capillary residual trapping](../../../../../../capillary-residual-trapping.md). The broken printed reference “(??)” points to the preceding outer profile.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
