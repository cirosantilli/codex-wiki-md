<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a fixed input the production terms are constant, so both [linear ordinary differential equations](../../../../../linear-ordinary-differential-equation-split.md) can also be solved exactly:

$$
\boxed{Y(t)=Y^*+[Y(0)-Y^*]e^{-t},\qquad
Z(t)=Z^*_{\rm direct}+[Z(0)-Z^*_{\rm direct}]e^{-t}}.
$$

Each displacement from its [equilibrium concentration](../../../../../equilibrium-concentration.md) decays with time constant one. The [Jacobian matrix](../../../../../jacobian-matrix.md) is $-I$, with two [eigenvalues](../../../../../eigenvalue.md) equal to $-1$, so the [fixed point](../../../../../fixed-point.md) is globally asymptotically stable for the nonnegative state space.

Here is a numerical solver using the [classical fourth-order Runge-Kutta method](../../../../../classical-fourth-order-runge-kutta-method.md); it uses only the repository's existing NumPy and matplotlib dependencies. Continue the definitions from part (b):

```
def integrate(rhs, initial, times):
    out = np.empty((len(times), len(initial)))
    out[0] = initial
    for j, dt in enumerate(np.diff(times)):
        state = out[j]
        k1 = rhs(state)
        k2 = rhs(state + dt*k1/2)
        k3 = rhs(state + dt*k2/2)
        k4 = rhs(state + dt*k3)
        out[j+1] = state + dt*(k1 + 2*k2 + 2*k3 + k4)/6
    return out

def direct_rhs(state, X):
    Y, Z = state
    return np.array([2*hill(X, 1, 2) - Y,
                     3*hill(X, 2, 4) - Z])

times = np.linspace(0, 8, 801)
plt.figure(figsize=(7, 4))
for initial, style in [([0, 0], "-"), ([3, 4], "--")]:
    trajectory = integrate(lambda s: direct_rhs(s, 2), initial, times)
    exact = np.array([1.6, 1.5]) + (np.array(initial) - [1.6, 1.5]) \
            * np.exp(-times[:, None])
    assert np.max(np.abs(trajectory - exact)) < 1e-8
    plt.plot(times, trajectory[:, 0], style, label=f"Y, initial {initial}")
    plt.plot(times, trajectory[:, 1], style, label=f"Z, initial {initial}")
plt.xlabel("Time")
plt.ylabel("Concentration")
plt.legend()
plt.tight_layout()
plt.show()
```

For $X=2$, **$\boxed{Y^*=1.6,\quad Z^*_{\rm direct}=1.5}$**. The initial state $(0,0)$ approaches those values from below, while $(3,4)$ approaches from above. Over eight time units the initial displacement is reduced by $e^{-8}\approx0.000335$, explaining why both trajectories nearly coincide with the equilibria from part (b). The two-panel figure above displays these simulations.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
