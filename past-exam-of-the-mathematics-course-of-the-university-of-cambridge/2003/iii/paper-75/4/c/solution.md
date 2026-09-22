<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the small-$\lambda$ and large-$\widetilde L$ limits at fixed $C$ first, then expand in small $C$. Seek $H=H_0+\lambda H_1+\cdots$. The leading equation is $H_{0X}=X$, so

$$
\boxed{H_0=\frac12(b^2+X^2)},\qquad b>0.
$$

At the next order,

$$
H_{1X}=H_0^{-3}-H_0^{-2}.
$$

For large $\widetilde L$, extend the integrals determining the localized film resistance to the whole line. The even leading profile has equal end values, so the [force](../../../../../../force.md) condition at order $\lambda$ becomes

$$
I_2-I_3=C\left(\frac43I_1-I_2\right),\qquad I_n=\int_{-\infty}^{\infty}H_0^{-n}\,dX.
$$

The left side follows from $H_1(-\widetilde L)-H_1(\widetilde L)=-\int H_{1X}\,dX$. Using the supplied integrals gives $I_1=2\pi/b$, $I_2=2\pi/b^3$, $I_3=3\pi/b^5$. Hence

$$
2b^2-3=C\left(\frac83b^4-2b^2\right).
$$

This fixes the integration constant in $H_0$. In terms of $z=b^{-2}$ it reads $2z-3z^2=C(8/3-2z)$. The root near $z=2/3$ gives

$$
\boxed{\frac1{b^2}=\frac23(1-C)+O(C^2)}.
$$

**The correction has a minus sign.** The printed $1+C$ is inconsistent with the supplied differential equation and [force](../../../../../../force.md) condition: substituting $z=(2/3)(1+C)$ gives $2z-3z^2=-(4/3)C+O(C^2)$, whereas $C(8/3-2z)=(4/3)C+O(C^2)$. The discrepancy is not a choice of flux sign, because the positive-gap scaling here requires $s=2Q/U>0$. The leading value $b^{-2}=2/3$ is unaffected by this error.

Use the [force](../../../../../../force.md) integral to calculate the leading [pressure](../../../../../../pressure.md) drop, retaining its first nonzero order in both $C$ and $\lambda$:

$$
\Delta p=\alpha sC\lambda\left(\frac43I_1-I_2\right)+\cdots.
$$

At $b^2=3/2$, the bracket is $4\pi/(3b)$. With the definitions of $C$ and $\lambda$ this gives the [small-speed compliant-plug lubrication asymptotics](../../../../../../small-speed-compliant-plug-lubrication-asymptotics.md)

$$
\boxed{\Delta p\simeq\frac{8\pi\sqrt{2/3}\,\mu U}{a\sqrt\kappa\,(2Q/U)^{1/2}}}.
$$

Thus the requested leading pressure-drop expression remains valid despite the sign error in its subsidiary correction.

Finally, the absolute downstream [pressure](../../../../../../pressure.md) selects $s$ and hence $Q/U$. At the downstream matching region the leading shape gives

$$
p_d-p_0\simeq\alpha\left[r_{00}-a+\frac{s b^2}{2}\right],
$$

because $sX^2/2$ cancels the unstressed parabolic term. For example, if the downstream excess [pressure](../../../../../../pressure.md) is fixed and

$$
d=\frac{p_d-p_0}{\alpha}-(r_{00}-a)>0,
$$

then $s\simeq2d/b^2\simeq4d/3$, and

$$
\boxed{\Delta p\simeq\frac{4\pi\sqrt2\,\mu}{a\sqrt{\kappa d}}\,U}.
$$

This is a linear pressure-speed law on the specified small-$\lambda$ branch. If $p_d-p_0$ depends on speed or cell state, its relation must instead be substituted to obtain the corresponding law. If $d\leq0$, the stated leading positive-gap branch does not exist. Without the absolute-pressure relation, the problem gives a family parameterized by $Q/U$, rather than a unique $\Delta p(U)$. Errors from finite $\widetilde L$, higher powers of $\lambda$ and higher powers of $C$ have been omitted consistently in this leading approximation. Resolving the displayed $O(C)$ correction to $b^{-2}$ requires the omitted finite-domain and higher-$\lambda$ corrections to be smaller than $C$; otherwise only its leading value is justified.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
