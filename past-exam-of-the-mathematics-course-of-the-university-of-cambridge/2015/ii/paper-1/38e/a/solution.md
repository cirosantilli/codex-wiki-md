<h1 id="38e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let all spatial [derivatives](../../../../../../derivative.md) be evaluated at $x=mh$, $t=nk$. Expand the two adjacent flux contributions symmetrically. The bracket in the scheme is

$$
S=a(x-h/2)[u(x-h)-u(x)]+a(x+h/2)[u(x+h)-u(x)]
=h^2(au_x)_x+O(h^4).
$$

For clarity, the $h^2$ terms are $au_{xx}+a'u_x$; odd orders cancel under $h\mapsto-h$. Under four spatial [derivatives](../../../../../../derivative.md) the next coefficient is $au_{xxxx}/12+a'u_{xxx}/6+a''u_{xx}/8+a^{(3)}u_x/24$. Time expansion gives $u(x,t+k)=u+k u_t+O(k^2)$. Since $u_t=(au_x)_x$ and $k=\mu h^2$,

$$
u(x,t+k)-u(x,t)-\mu S=O(k^2)+O(\mu h^4)=\boxed{O(h^4)}.
$$

This stronger smooth-data residual implies the requested **$O(h^3)$** consistency bound. Even a less detailed Taylor expansion with an $O(h^3)$ spatial remainder would suffice for the printed order. Uniform bounds on the needed [derivatives](../../../../../../derivative.md) over the region under consideration make the estimate uniform in the interior mesh index; the zero boundary values enter the scheme exactly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38E](../../38e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
