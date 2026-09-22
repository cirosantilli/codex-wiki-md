# Scalar static-state Kalman update

↑ **Parent:** [Kalman filter](kalman-filter.md)

Suppose $x\mid\mathcal F\sim N(\widehat x,V)$ and the new observation is $y=x+\eta$, where $\eta\sim N(0,R)$ is independent. Then

$$
\mathbb E[x\mid\mathcal F,y]
=\widehat x+\frac{V}{V+R}(y-\widehat x),
\qquad
\operatorname{Var}(x\mid\mathcal F,y)
=\frac{VR}{V+R}.
$$

The coefficient $V/(V+R)$ is the scalar Kalman gain.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/30k/a/solution.md)
