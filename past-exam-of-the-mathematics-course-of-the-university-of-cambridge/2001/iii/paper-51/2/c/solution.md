<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the nonzero [stationary branch of five-mode magnetoconvection](../../../../../../stationary-branch-of-five-mode-magnetoconvection.md), put $s=a^2$ and $m=(4-\varpi)\zeta^2/\varpi>0$. The temperature equations first give $b=a/(1+s)$ and $c=s/(1+s)$. The magnetic equations then give

$$
e={s\over m+s},\qquad d={ma\over\zeta(m+s)}.
$$

Divide the steady first equation by $\sigma a$ and substitute these expressions. The exact branch is

$$
\boxed{r(s)=(1+s)\left[1+{qm[m+(4-\varpi)s]\over(m+s)^2}\right].}
$$

Expanding at $s=0$ gives

$$
\boxed{r=1+q+r_2a^2+O(a^4),\qquad r_2=1+q+{q\varpi(2-\varpi)\over(4-\varpi)\zeta^2}.}
$$

Near $\varpi=2$ the required amplitude restriction $a^2\ll\zeta^2$ ensures $s\ll m$. For $\varpi\le2$, $r_2>0$, so the paired [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) emerge in the forward direction $r>1+q$. For fixed $q>0$ and small $\zeta$, the [pitchfork reversal near geometric ratio two in magnetoconvection](../../../../../../pitchfork-reversal-near-geometric-ratio-two-in-magnetoconvection.md) occurs at

$$
\boxed{\varpi_c=2+{1+q\over q}\zeta^2+O(\zeta^4).}
$$

This follows by expanding the exact zero-slope equation $q\varpi(2-\varpi)+(4-\varpi)\zeta^2(1+q)=0$. Above this value the branch initially runs backwards into $r<1+q$; at $q=0$ there is no reversal. This is a degenerate [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) at $r_2=0$, not a conclusion that every emerging state is stable. If $B_s>0$, the center-direction cubic term has the opposite sign to $r_2$: the forward branch is locally attracting and the backward branch repelling. If $B_s<0$, an unstable transverse mode remains.

For the nearby geometry, the next coefficient is $r_4=q[(2\varpi-5)/m^2+(2-\varpi)/m]$, which is negative near the reversal. Thus a small positive $r_2$ produces a nearby maximum of $r$ at $s\simeq-r_2/(2r_4)>0$; this fold approaches the pitchfork as $r_2\downarrow0$. Once $r_2<0$ the small-amplitude branch is backward. The exact formula eventually grows like $r\sim s$, so a backward branch must turn at a finite amplitude, potentially outside the small-amplitude expansion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
