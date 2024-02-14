CURRENT, RESISTANCE, AND OHM'S LAW
==================================

Current
-------

Electrical circuits --- lighting our homes, powering our phones, and controlling our own thoughts and actions in neural networks --- are driven by moving charge.

Consider an electric field passing through a metal cylinder:

![An upward vertical electric field passing through metal cylinder; negative charges experiencing downward electric force](images/07_Efield_through_metal.png)

- Free electrons will feel a force (opposite to the direction of $\vec{E}$, since $q_e = -e$)

- If the cylinder is allowed to come to equilibrium, the electrons will arrange themselves such that the electric field inside the conductor is zero (the "static" or equilibrium case we have already discussed) with a build-up of negative charge on the bottom.

![An upward vertical electric field passing through metal cylinder, driven by wireand electromotive force; negative charges experiencing downward electric force](images/07_Efield_through_metal_circuit.png)

- If, however, another conductor (a wire) is attached, connecting the two ends of the cylinder, then the system will *not* come to equilibrium and electrons will flow in a loop or circuit.

- The flow rate of charge going past any cross-section of the conductor is called the **current**.

Since there is a force, $\vec{F}_E$, on the electrons, one might think that they accelerate (moving faster and faster around the circuit. In fact, they do not:

![Random thermal motion of electrons in a wire](images/07_thermal_motion_electrons_wire.png)

- At any nonzero temperature ($T>0$ K), the primary motion of electrons is *thermal*: fast and randomly-directed ($v_\text{th} \sim 10^5$ at room temperature).

- Electrons ove a very short distance before *colliding* with the metal's lattice of nuclei.

The electric force on free electrons in a conductor serves to change the thermal velocities very slightly, causing a small drift velocity, $v_d$, of electrons in the direction of the force.

![Random thermal motion of electrons in a wire, but slightly adjusted due the electric force of an electric field, causing a drift velocity opposing the field.](images/07_thermal_motion_electrons_w_field.png)

- The drift velocity, even for large currents is very small: $v_d \sim 10^{-5}$ m/s $\ll v_\text{th} \sim 10^5$ m/s.

- Question: What is $v_d$ in cm/h?

Definitions of Current (I), Current Density (Jvec), and Resistivity (rho)
------------------------------------------------------------------------

**Def'n**: Take a long conductor (call it a "wire") with an electric field directed along its length, and consider any cross-sectional area of the wire, $A$. The **current passing through $A$** is:
```math
I = \frac{\text{Net charge passing through $A$ in $\Delta t$}}{\Delta t}
```
The *direction* of the current is the direction of $\vec{E}$, i.e., the direction that positive charge carriers would flow. Given the presence of $\vec{E}$, positive charges will flow in one direction across $A$, and negative charge carriers will flow in the other direction.  Both of those will be considered a current in the direction of $\vec{E}$.  An equal amount of positive and negative charges passing the same way through A would yield a net charge flux of zero and therefore a zero current.  Although we give it a direction, the current, $I$, is not a vector.

![Current flow thorugh cross-sectional are with positive and negative charge carriers](images/07_current-flow-charge-carriers.png)

Examples:

![Current flow in neutral salt solution, acidic solution (excess +), and metal (free electrons)](images/07_three-example-current.png)

If we simplify to a single charge, $q$, with drift velocity, $v_d$, we can write the current as:
```math
\begin{align}
I &= \frac{|Q_\text{through A in $\Delta t$|}|}{\Delta t} = \frac{|q| N_\text{through A in $\Delta t$}}{\Delta t} = \frac{|q| n V_\text{through A in $\Delta t$}}{\Delta t} = \frac{|q| n A \Delta x_\text{in $\Delta t$}}{\Delta t} \\
& \rightarrow I = |q| n A v_d
\end{align}
```
where $n$ is the number of charge carriers per unit volume (called the *number density*, with $[n] = \text{m}^{-3}$).

![Drift velocity calculation of current](images/07_drift-velocity-current-calculation.png)

**Def'n**: Given an arbitrary conductor (no longer restricting ourselves to a "wire") with a penetrating electric field, $\vec{E}(\vec{r})$, one can imagine there will be a corresponding drift velocity field, $\vec{v}_d(\vec{r})$, meaning that, at every point $\vec{r}$, the charge carriers in that vicinity (let's assume a single type of charge carrier, with charge $q$) have an average drift velocity vector $\vec{v}_d$.  We can therefore define the **current density field**, $\vec{J}(\vec{r})$, as the current per unit area ($|\vec{J}| = I/A$) at every point:
```math
\vec{J}(\vec{r}) := q n \vec{v}_d(\vec{r}).
```
Since, for positive charge carriers, the drift velocity points in the same direction as $\vec{E}$, we can write this as
```math
\vec{J} = \sigma \vec{E} = (1/\rho) \vec{E}
```
where we have defined $\sigma$ as the **conductivity** of the material and $\rho$ as the **resistivity** (the inverse of the conductivity). Note that neither of these are "charge densities" (like we saw a few units ago), they just use the same symbol. The equation above is the most basic expression of "Ohm's Law" (see below).

We will primarily use the current, $I$, rather than the current density, $\vec{J}$. They are related by:
```math
I = \int_S \vec{J} \cdot d\vec{A} = \int_S \vec{J} \cdot \hat{n} dA
```
meaning that the current is the flux of the current density through a chosen surface, $S$.

![Flux of the current density field](images/07_flux-of-current-density.png)


"Electromotive Force" (EMF) and Batteries
------------------------------------------------------------------------

Ohm's Law and Resistance
------------------------------------------------------------------------

A Simple Circuit
------------------------------------------------------------------------

Energy in Electric Circuits
------------------------------------------------------------------------