# Scalar delayed-observation LQG regulator

↑ **Parent:** [Optimal control](optimal-control.md)

For $X_{n+1}=X_n+U_n+\varepsilon_{n+1}$ and $Y_{n+1}=X_n+\eta_{n+1}$ with independent unit-variance normal noises, the equilibrium prediction-error variance is $P=(1+\sqrt5)/2$. Orthogonality to the next innovation gives the filtering gain $H=P/(1+P)$. Minimizing the quadratic average cost gives a control Riccati coefficient $R$ satisfying $R^2=R+1$, so $R=P$ and $K=R/(1+R)=H$. Completing the control square yields minimal cost $R+(1+R)K^2P=1+\sqrt5$. The one-step observation delay is essential to the value of $P$.

## ↑ Ancestors (5)

1. [Optimal control](optimal-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/29i/solution.md)
