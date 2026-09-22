<h1 id="3/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $H(a,b)=|a-b|$ and $Q(a,b)=\operatorname{sgn}(a-b)(f(a)-f(b))$. Both are symmetric in $a,b$. For fixed $(s,y)$ apply the entropy inequality for $u$ at the constant level $k=v(s,y)$ with test $\Phi(t,x,s,y)$, then integrate over $(s,y)$. This produces

$$
\int H(u,v)\Phi_t+Q(u,v)\Phi_x+\int H(u_0(x),v(s,y))\Phi(0,x,s,y)\ge0.
$$

Here the first integral is over both time-space pairs and the second over the three remaining variables. Repeat with $v$, level $u(t,x)$, integrating over $(t,x)$, to obtain the analogous terms with $\Phi_s,\Phi_y$ and initial value $v_0$.

Adding and using symmetry gives

$$
\boxed{\int\bigl[H(u,v)(\Phi_t+\Phi_s)+Q(u,v)(\Phi_x+\Phi_y)\bigr]+B_u+B_v\ge0,}
$$

where $B_u=\int H(u_0(x),v(s,y))\Phi(0,x,s,y)\,ds\,dx\,dy$ and $B_v=\int H(u(t,x),v_0(y))\Phi(t,x,0,y)\,dt\,dx\,dy$. All integrals are finite on the test's compact support because the states are bounded. The levels being inserted are constants relative to the variables in each entropy inequality; there is no differentiation of the merely measurable other solution. [Fubini's theorem](../../../../../../../fubini-s-theorem.md) and continuity of $H,Q$ justify the integration. This is [doubling of variables for scalar conservation laws](../../../../../../../doubling-of-variables-for-scalar-conservation-laws.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
