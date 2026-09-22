<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A nonidentity [transvection](../../../../../../transvection.md) is a linear automorphism $\tau=I+N$ with $\operatorname{rank}N=1$ and $N^2=0$. Equivalently, it fixes a [hyperplane](../../../../../../hyperplane.md) pointwise and its displacement has image in a line lying in that hyperplane. The notation $T\setminus\{1\}$ allows the identity as a degenerate [transvection](../../../../../../transvection.md); use that convention here, with $N=0$ also allowed.

For a nonidentity [transvection](../../../../../../transvection.md), choose $d\ne0$ spanning the image of $N$. There is a unique nonzero [linear functional](../../../../../../linear-functional.md) $f$ such that $N(v)=f(v)d$. Since $N^2(v)=f(v)f(d)d$, we have $f(d)=0$, so $d\in\ker f$. Conversely, this condition makes $(df)^2=0$ and gives inverse $I-df$. The identity is represented by $f=0$ and any $d\ne0$. Thus

$$
\boxed{\tau_{f,d}(v)=v+f(v)d,\qquad d\ne0,\quad f(d)=0.}
$$

When $f(d)=f'(d)=0$, the two displacement maps have zero product, giving

$$
\boxed{\tau_{f,d}\tau_{f',d}=\tau_{f+f',d},\qquad \tau_{f,d}^{-1}=\tau_{-f,d}.}
$$

For clarity use left actions of linear maps. Applying $g^{-1}$, then $\tau_{f,d}$, then $g$ gives

$$
\boxed{g\tau_{f,d}g^{-1}=\tau_{f\circ g^{-1},\,g(d)}.}
$$

With the alternative conjugation notation $\tau^g=g^{-1}\tau g$, the answer is $\tau_{f,d}^g=\tau_{f\circ g,\,g^{-1}(d)}$. In either convention the transformed direction lies in the kernel of the transformed functional.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
