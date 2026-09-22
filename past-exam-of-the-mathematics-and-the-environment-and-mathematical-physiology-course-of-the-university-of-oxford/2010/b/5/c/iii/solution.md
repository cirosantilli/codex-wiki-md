<h1 id="b/5/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $c_\uparrow(w)$ denote the increasing-front speed from the preceding solution. Reversing that heteroclinic reverses its speed, so a decreasing back has speed $c_\downarrow(w)=-c_\uparrow(w)$. A rigidly travelling pulse has one speed throughout, requiring

$$
\boxed{c=c_\uparrow(0)=c_\downarrow(w_0),\qquad c_\uparrow(w_0)=-c_\uparrow(0).}
$$

This is the correct use of the integral formula: compare the oppositely oriented transitions, including their signs, rather than equating two increasing-front speeds.

For completeness, write $f(v)-w=-(v-r_1)(v-r_2)(v-r_3)$, $r_1<r_2<r_3$. The explicit increasing [frozen-recovery cubic front](../../../../../../frozen-recovery-cubic-front.md) is

$$
v(X)=r_1+\frac{r_3-r_1}{1+\exp[-(r_3-r_1)X/\sqrt2]},\qquad c_\uparrow(w)=\frac{r_1+r_3-2r_2}{\sqrt2}.
$$

Substitution, using $v_X=(v-r_1)(r_3-v)/\sqrt2$, verifies the equation. Since $r_1+r_2+r_3=1+a$, speed matching gives

$$
c_\uparrow(0)=\frac{1-2a}{\sqrt2},\qquad r_2(w_0)=\frac{2-a}{3},\qquad\boxed{w_0=f\!\left(\frac{2-a}{3}\right)=\frac{2(2-a)(1-2a)(1+a)}{27}.}
$$

For $0<a<1/2$ this selects the appropriate positive back level within the cubic's three-root range. The high branch connects $B$ to $C$ slowly, and the low branch supplies recovery after $D$.

**The stated positive-speed, rising-front orientation imposes $a<1/2$ at leading order.** The printed range $0<a<1$ by itself does not guarantee that pulse construction: at $a=1/2$ the leading front is stationary, while for $a>1/2$ the calculated increasing-front speed is negative. Existence and stability of a full finite-$\epsilon$ pulse also require the slow connections; speed matching is its leading necessary construction, rather than a proof for every parameter in the printed range.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../split.md)
7. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
