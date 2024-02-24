# Magnets, Magnetic Fields, and Magnetic Forces

## Magnets and Magnetism

### Basic Properties of Magnets

![A classic bar magnet with a "north" and a "south" pole.](images/10_bar-magnet.png)

* Magnets are intrinsically **dipolar**, having a "North" and a "South" **pole**.
* Magnetic dipoles cannot be divided into N/S monopoles, cutting a magnet in two creates two magnets:

![Bar magnet cut in half yields two bar magnets.](images/10_cutting-bar-magnet.png)

* There are **attractive/repulsive forces** between opposite/same poles:

![Like poles of two magnets repel. Opposite poles attract](images/10_attract-repel-bar-magnet.png)

* A magnet has a surrounding magnetic field (more later).

![A compass needle is a magnet.  It aligns with the magnetic field of the earth and points toward geographic North.](images/10_geomagnetic-north-compass.png)

* A magnet (e.g., a compass needle) will *align* in the magnetic field of another magnet (e.g., the Earth). (There is a torque on a magnetic dipole causing this alignment, we will not explore this further).


### Magnetic Materials

![A current loop creates a magnetic dipole field (next time).](images/10_current-loop-dipole.png)

We will see in the next lecture that moving charge (or current) creates a magnetic field. Magnetic materials (magnets) have a magnetic field because of moving charge on the atomic level.

![Electrons orbiting the nucleus of an atom cause orbital currents creating magnetic fields, but also have an intrinsic "spin" creating a magnetic field](images/10_orbital-dipoles-spin.png)

There are two types of atomic-scale magnetic dipoles, due to:
1. "Orbital motion" of the electron about the nucleus,
2. "Spin" — an intrinsic magnetic dipole characteristic of electrons.

Note: At this small scale, these effects are necessarily quantum. Moving/spinning charge is a convenient metaphor, but an inaccurate description.

![A horseshoe magnet can cause a magnetic material to have its own magnetic field](images/10_horseshoe-magnetization.png)

A material is said to be **magnetic** if it has a net atomic dipole (due to, e.g., unpaired valence electrons) that can align with an external magnetic field.

![Ferromagnetic materials have "domains" of aligned magnets](images/10_magnetic-domains.png)

So-called "Permanent Magnets" are made from **ferromagnetic8* materials. These have large atomic dipoles and the ability to form large domains of aligned dipoles in the presence of an external magnetic field. These domains remain when the external field is removed.

![Iron and its unpaired electrons make it an archtypal ferromagnetic material](images/10_iron-unpaired-electrons.png)

If a ferromagnetic material is heated above a critical temperature (the **Curie temperature**) it loses the ability to form domains (and thus lasting magnetism). These materials are called **paramagnetic**.


## Magnetic Field

Just as we defined the electric field through the force on a test charge, we will define magnetic field direction by the alignment of magnets within it.

![A compass needle, which is a bar magnet itself, aligning in an external magneetic field B](images/10_compass-B-field.png)

The **magnetic field at a point in space** points in the direction of a magnet's alignment (e.g., a compass needle).

**Magnetic field lines** are continuous lines which are everywhere parallel to the magnetic field.

We can probe the space around a magnet with a compass to determine the magnetic field at each point in space (see below)

### Magnetic field lines of a bar magnet

![Using a compass to explore the magnetic field of a bar magnet (left) and the resulting magnetic field lines (right)](images/10_compasses-B-field-bar-magnet.png)

### Magnetic field of the Earth

Compasses can also be used to probe the **magnetic field of the Earth**. In our classroom in Allendale, MI, compasses restricted to the horizontal and vertical planes shown:

![We can identify the magnetic field vector at our point on Earth (Allendale, MI), using a horizontal and a vertical compass](images/10_magnetic-field-earth-in-classroom.png)

These probes indicate that the magnetic field points down into the Earth, with a component pointing toward our geographic North Pole.

If we put this on a globe and assume some symmetry...

![Using the direction of the magnetic field at one point on the Earth (Allendale) we can extrapolate what the field looks like at other points, assuming symmetry](images/10_magnetic-field-of-earth.png)

Based on the field lines drawn, you can sketch the "bar magnet that sits inside the Earth" to create this field (do it!). The field actually flips its polarity every 100,000 years or so, and we don’t actually know exactly what creates the field or its dynamics.

## Magnetic Force on a Moving Charge or Current

A current-carrying wire in a magnetic field will experience a force in a direction perpendicular to both the wire and the field lines, a charged particle moving in a magnetic field will experience a force perpendicular to its velocity and the field.

The **force on a moving charge** is proportional to the charge, the field strength and the particle speed. Therefore:
```math
\vec{F}_B = q\vec{v} \times \vec{B}
```
where this **cross product** of vectors means that the magnitude is:
```math
|\vec{F}_B| = |q||\vec{v}||\vec{B}|\sin\theta_{vB}
```
and the direction of the force is given by the **right hand rule**:

1. Point the fingers of your right hand along the first vector $\vec{v}$.
2. Close your fingers in the direction of the second vector $\vec{B}$.
3. The resulting vector $\vec{F}_B$ points in the direction of your thumb.

![How to use the right-hand rule to determine the force on a moving charge in a magnetic field, B.](images/10_right-hand-rule-B-force.png)

Note from the basic equation for $\vec{F}_B$, however, that a negative charge, $q<0$, will experience a force in the opposite direction to what is found in the picture.
