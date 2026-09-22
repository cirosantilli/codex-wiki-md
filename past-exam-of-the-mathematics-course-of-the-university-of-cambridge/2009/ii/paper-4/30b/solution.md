<h1 id="30b/solution">Solution</h1>

↑ **Parent:** [30B](../30b.md)

Write the [Fourier coefficients](../../../../../fourier-coefficient.md) of the two boundary functions as $a_{j,n}=(2\pi)^{-1}\int_0^{2\pi}u_j(\varphi)e^{-in\varphi}\,d\varphi$. The [Laplace equation](../../../../../laplace-equation.md) in polar coordinates is $u_{rr}+r^{-1}u_r+r^{-2}u_{\varphi\varphi}=0$. A separated mode $R(r)e^{in\varphi}$ satisfies $r^2R''+rR'-n^2R=0$. The ansatz $R=r^\alpha$ gives $\alpha^2=n^2$, so the solutions are $r^{|n|},r^{-|n|}$ for $n\ne0$ and $1,\log r$ for $n=0$.

Set $s=\log(r/R_1)$ and $L=\log(R_2/R_1)$. Solving the two boundary equations for every mode yields

$$
\boxed{u(r,\varphi)=a_{1,0}\left(1-\frac sL\right)+a_{2,0}\frac sL
+\sum_{n\ne0}\left[a_{1,n}\frac{\sinh(|n|(L-s))}{\sinh(|n|L)}
+a_{2,n}\frac{\sinh(|n|s)}{\sinh(|n|L)}\right]e^{in\varphi}.}
$$

For real boundary data, the conjugate coefficients ensure this is real. On any compact subannulus $0<\delta\le s\le L-\delta$, the multipliers and all their differentiated versions are bounded by a [polynomial](../../../../../polynomial-split.md) in $|n|$ times $e^{-\delta|n|}$. The boundary coefficients are square summable by [Parseval identity](../../../../../parseval-identity.md), so [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) proves locally uniform convergence of the series and of all its derivatives. Thus it is smooth and satisfies the [Laplace equation](../../../../../laplace-equation.md) term by term.

Because the data are only $L^2$, the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) is interpreted in $L^2$ on circles. As $s\downarrow0$, the first multiplier tends to one and the second to zero; both lie between zero and one. Dominated convergence of the square-summable [Fourier coefficients](../../../../../fourier-coefficient.md) gives $u(r,\cdot)\to u_1$ in $L^2$, and similarly $u\to u_2$ as $s\uparrow L$. Finally, any harmonic solution with these $L^2$ traces has [Fourier coefficients](../../../../../fourier-coefficient.md) satisfying the radial equation above with the same two endpoint values. Uniqueness of those scalar boundary-value problems makes every coefficient equal to the displayed one. Hence **this is the unique harmonic solution with the prescribed $L^2$ traces**; pointwise values at every boundary angle are not required by the given data.

## ↑ Ancestors (10)

1. [30B](../30b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
