# Equipotential Surfaces and Capacitance

## Equipotential Surfaces

Last time we defined the change in potential as
   ```math
   \Delta V = \frac{\Delta U_e}{q_{\text{test}}} = \frac{-W_e}{q_{\text{test}}}
   ```
Meaning that the change in potential from one point in an electric field to another is found by calculating the change in potential energy (U) when moving a test charge between those two points, and dividing by that charge.

The work is being done by the force of the electric field, $\vec{F}_e = q_e \vec{E}$, so we can write
```math
\begin{align}
\Delta V & = \frac{-W_e}{q_{\text{test}}} = \frac{-\vec{F}_e \cdot \Delta \vec{s}}{q_{\text{test}}} = \frac{-q_{\text{test}} \vec{E} \cdot \Delta \vec{s}}{q_{\text{test}}}\\
& \Rightarrow \Delta V = - \vec{E} \cdot \Delta \vec{s}
```
(For a uniform electric field, this is the same as our expression: $\Delta V = -Ed$)

Recall that the "dot product" is:
```math
\vec{A} \cdot \vec{B} = AB \cos \theta_{AB}
```
Meaning that it is:

- Positive when $\vec{A}$ & $\vec{B}$ in "same direction" ($0 \leq \theta_{AB} < 90^\circ$)
- Zero when $\vec{A} \perp \vec{B}$ ($\theta_{AB} = 90^\circ$)
- Negative when $\vec{A}$ & $\vec{B}$ point in "opposite dir." ($90^\circ < \theta_{AB} \leq 180^\circ$)

So, the change in potential, $\Delta V$, is:

- Negative when moving along the E-field lines
- Zero when moving perpendicular to the E-field
- Positive when moving against the E-field lines
