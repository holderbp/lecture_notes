
# Ampere's Law

## Introduction

As mentioned last lecture, we return to Maxwell's Equations to find a piece that describes the magnetic field created by currents. The full equation, and the piece we consider today is:
```math
\nabla \times \vec{B} = \mu_0 \frac{\partial \vec{E}}{\partial t} + \mu_0 \vec{J} \quad \rightarrow \quad \nabla \times \vec{B} = \mu_0 \vec{J} 
```
So, we are ignoring changing electric fields ($\partial \vec{E} / \partial t = 0$) for the moment and considering only how magnetic fields relate to current density, $\vec{J}$.

We will now convert this equation from the entirely foreign mathematical language of partial derivative operators ($\nabla \times \vec{B}$ is called the "curl" of the vector field $\vec{B}$), into the slightly more familiar language of line integrals. We do this in almost the same way we dealt with Gauss's Law in the third lecture, i.e., by taking an integral. Recall that we did this:

![Manipulation of Gauss's law from differential form to integral form](images/13_gauss-law-derivation-schematic.png)

```math
\nabla \cdot \vec{E} = \frac{\rho}{\varepsilon_0} \quad \rightarrow \quad
\oint_{S = \partial R} \vec{E} \cdot \hat{n} \,dA = \frac{Q_{\text{enc}}}{\varepsilon_0} 
```
In words: we took a volume integral of both sides over some region of space $R$, on the right-hand side that gave us the sum of all charge in the region (or the "charge enclosed" by the boundary surface $S = \partial R$), and on the left-hand side we used a theorem to write the volume integral of the divergence as the flux of the electric field through the bounding surface $S$ (the so-called "Gaussian surface"). 

Before making a similar transformation of Ampere's Law, let's do exactly the same transformation of another one of Maxwell's Equations:
```math
\nabla \cdot \vec{B} = 0 \quad \rightarrow \quad \oint_R \nabla \cdot \vec{B} \, dV = \oint_R 0 \, dV \quad \rightarrow \quad \oint_{S = \partial R} \vec{B} \cdot \hat{n} \, dA = 0
```

This law, "Gauss's Law for Magnetic Fields," tells us that the flux of the magnetic field through any closed surface is zero. We have seen this in all of our pictures of magnetic fields ... all field lines "close," similarly to the electric field lines of an electric dipole.

![Comparing Gauss law for electric vs magnetic fields](images/13_positive-vs-zero-flux.png)

But, there is a big difference... For the magnetic field, no field lines *originate* within the "gaussian surface" $S$.  **There are no magnetic monopoles** (no "magnetic charge").

So, let us now convert Ampere's law. This time we will make use of a different theorem, called Stoke's theorem, which says that the flux of the curl of a vector field, $\vec{F}(t)$, through some 2D surface, $S$, is equal to the line integral around the closed loop of its boundary, i.e., $\partial S = \delta S$. In equations:
```math
\Phi_{\vec{\nabla} \times \vec{F}} = \iint_{S} (\nabla \times \vec{F}) \cdot \mathrm{d}\vec{A} = \oint_{C=\partial S} \vec{F} \cdot \mathrm{d}\vec{r} = \oint_{C} \vec{F} \cdot \vec{v} \mathrm{d}t \quad \quad \text{Stoke's Theorem}
```
where we write $\vec{v}$ as $\frac{\mathrm{d}\vec{r}}{\mathrm{d}t}$.

So, we rewrite the differential form of Ampere's Law:
```math
\begin{align}
\nabla \times \vec{B} &= \mu_0 \vec{J}
\int_{S} (\nabla \times \vec{B}) \cdot \hat{n} \, dA & = \int_{S} \left(\mu_0 \vec{J}\right) \cdot \hat{n} \, dA \\
\oint_{C=\partial S} \vec{B} \cdot \mathrm{d}\vec{r} & = \mu_0 \iint_{S} \vec{J} \cdot \hat{n} \, dA\\
\oint_{C=\partial S} \vec{B} \cdot \mathrm{d}\vec{r} & = \mu_0 \, I_\text{through $S$}
\end{align}
```
This equation will play the role that Gauss's Law did for electric fields: it will connect the magnetic field in space to its source, current flow. Similar to Gauss's Law, the equation is always true, but only yields a useful and easy calculation for systems with a lot of symmetry.

### Example: Long, straight, current-carrying wire.

Just as we did for Gauss's Law, we will need to apply symmetry arguments to understand the basic picture of the magnetic field $\vec{B}$ and to compute exactly because problems with Ampere's Law. For a long, straight, current-carrying wire, we know that the rotational symmetry of the wire about an axis along it means that $\vec{B}$ has the same magnitude at all points on an enclosing circle.

![Figure demonstrating rotational symmetry of long straight wire](images/13_symmetry-long-straight-wire.png)

Because the wire and its current are unchanged under rotation, and because the magnetic field they produce must have the same symmetry, it must be true that:
```math
| \vec{B} \left(\vec{r}_1\right)| = | \vec{B} \left(\vec{r}_2\right)| = | \vec{B} \left(r \right)|
```
for any two points with $|\vec{r}_1| = | \vec{r}_2 | = r$, i.e., any two points on that circle.

It turns out that arguing for the *direction* of $\vec{B}$ on that circle is harder than it was for $\vec{E}$, so we will simply accept our prior knowledge from the right-hand rule applied to Biot-Savart ( $\vec{B}$ points tangent to the circle).

(Note: Some details about it being "harder". It is related to $\vec{B}$ being a so-called "pseudovector", which acquires a minus sign (a flip into the opposite direction) for any reflectional transformation.)



