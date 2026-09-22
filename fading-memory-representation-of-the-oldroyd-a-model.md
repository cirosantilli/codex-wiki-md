# Fading-memory representation of the Oldroyd-A model

↑ **Parent:** [Oldroyd-A model](oldroyd-a-model.md)

Put $S=\sigma^d-2\mu_rD$ in the [Oldroyd-A model](oldroyd-a-model.md). It obeys $\mathcal D_lS+S/\tau=2(\mu-\mu_r)D/\tau$. Pulling back as $F^TSF$ converts this to an ordinary linear relaxation equation. With decayed remote-past initial memory, its solution is

$$
\sigma^d(t)=2\mu_rD(t)+\frac{2(\mu-\mu_r)}\tau\int_{-\infty}^t e^{-(t-s)/\tau}F(t)^{-T}F(s)^TD(s)F(s)F(t)^{-1}\,ds.
$$

At a finite initial time, include the homogeneous transported term $e^{-(t-t_0)/\tau}F(t)^{-T}F(t_0)^TS(t_0)F(t_0)F(t)^{-1}$. The integral-only law is not equivalent to all arbitrary initial-value solutions without a memory condition.

## ↑ Ancestors (8)

1. [Oldroyd-A model](oldroyd-a-model.md)
2. [Viscoelasticity](viscoelasticity.md)
3. [Non-Newtonian fluid](non-newtonian-fluid.md)
4. [Rheology](rheology-split.md)
5. [Fluid mechanics](fluid-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-76/5/solution.md)
