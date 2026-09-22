<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Adding the three equations of the [SIRS model](../../../../../sir-model-with-waning-immunity.md) gives

$$
\frac d{dt}(S+I+R)=0,
$$

so

$$
\boxed{S(t)+I(t)+R(t)=N.}
$$

At a fixed point, $I(bS-c)=0$. The disease-free equilibrium is

$$
\boxed{(S,I,R)=(N,0,0).}
$$

For an endemic equilibrium $I^*>0$, one has $S^*=c/b$ and $aR^*=cI^*$. Conservation then gives

$$
\boxed{S^*=\frac cb,
\qquad I^*=\frac{a(bN-c)}{b(a+c)},
\qquad R^*=\frac{c(bN-c)}{b(a+c)}.}
$$

It exists with positive infected population exactly when

$$
\boxed{bN>c,}
$$

equivalently when the [basic reproduction number](../../../../../basic-reproduction-number.md) $bN/c$ exceeds one.

Eliminating $R=N-S-I$ yields

$$
\dot S=a(N-S-I)-bSI,
\qquad
\dot I=(bS-c)I.
$$

At the endemic equilibrium its [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}
-a-bI^*&-(a+c)\\
bI^*&0
\end{pmatrix}.
$$

Its trace and determinant are

$$
T=-\frac{a(a+bN)}{a+c}<0,
\qquad D=a(bN-c)>0.
$$

Therefore the endemic equilibrium is locally asymptotically stable. It is a stable node when

$$
\boxed{\frac{a^2(a+bN)^2}{(a+c)^2}\geq4a(bN-c),}
$$

and a stable focus when the inequality is reversed. Near a node, perturbations are sums of two nonoscillatory decaying exponentials. Near a focus, they execute damped oscillations with decay rate $-T/2$ and angular frequency $\sqrt{4D-T^2}/2$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
