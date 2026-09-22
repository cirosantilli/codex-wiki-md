<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Assume [Newton's second law](../../../../../newton-s-second-law.md), $F_{ij}=-F_{ji}$, and that each internal pair force is central, so $F_{ij}$ is parallel to $r_i-r_j$. Summing

$$
m_i\ddot r_i=F_i+\sum_{j\ne i}F_{ij}
$$

cancels internal pairs and gives $dP/dt=F:=\sum_iF_i$. Taking moments about fixed $a$ cancels the internal [torques](../../../../../torque.md) pairwise and gives

$$
\frac{dL}{dt}=G:=\sum_i(r_i-a)\times F_i.
$$

The [angular momentum about the centre of mass](../../../../../angular-momentum-about-the-centre-of-mass.md) result follows similarly: differentiating $\sum_i(r_i-R)\times m_i(\dot r_i-\dot R)$ introduces no extra term because both total relative position weighted by mass and total relative [momentum](../../../../../momentum.md) vanish. Thus its [derivative](../../../../../derivative.md) is the external [torque](../../../../../torque.md) about $R$.

Finally, if every mass is $m$ and $F_i=-k\dot r_i$, then about a fixed point

$$
G=-k\sum_i(r_i-a)\times\dot r_i=-\frac{k}{m}L.
$$

Therefore

$$
\boxed{L(t)=L(0)e^{-kt/m}.}
$$

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
