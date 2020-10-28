# <img alt="scientific-snap-icon" src="../../images/einstein_snap.png" width="50"/> Example: Stellar/Planetary Structure

In this example, we'll see how to derive the inner density structure of a star or planet by solving the equation of hydrostatic equilibrium using a simple model for the connection between the density and pressure - the "equation of state".

## Introduction

Of course, stars and planets are seemingly infinitely complicated objects full of exotic physical processes under conditions of temperature and density that can only be partically studied in Earthly laboratories.  On the other hand, the basics are actually quite simple: these bodies have lots of mass that produces lots of gravity that wants to compress the material into smaller and smaller volumes but the pressure differences within the hot gas resists the pull of gravity, resulting in a (usually) stationary state where the two forces are balanced.  This stable state is called "hydrostatic equilibrium".  Without gravity, the pressure differences in the object would cause the object to fly apart (e.g. in Earthly weather, the wind blows from high pressure regions to low pressure regions) and without the force due to pressure differences, the object would collapse to a Black Hole.

The "Equation of Hydrostatic Equilibrium" shows exactly how the two forces are balanced and can be derived from Newton's second law, Force = Mass\*Acceleration.

Let ![deltaP](./images/delta_P.png) be the difference in pressure between the lower and upper sides of a parcel of gas in a star or planet (only a difference in pressure produces a net local force, since the same pressure on both sides would be fully balanced and there would be no effect).

Let ![deltaA,deltar](./images/delta_A_delta_r.png) be the area perpendicular to the forces and the radial thickness (stars and planets are pretty spherical so all we need consider is the radial structure).

Let ![rho mass](./images/rho_mass.png) be the mass-density (e.g. in kg/m^3) and mass of the parcel.

Newton's Second Law then says that ![dF = dP dA = -dA dr rho a](./images/newton_2nd.png) (the minus sign comes in because gravity points downwards).  This equation is easily simplified to

![hydrostatic equilibrium](./images/hydrostatic_equilibrium.png)

This equation tells us that the force caused by a local radial gradient in pressure must be balanced by the gravitational force on material at the local density.

The gravitational acceleration is caused by all of the mass in the object at radii below the parcel (an amazing result found by Newton - the gravity of all the material at higher radii cancels out):

![gravity](./images/gravity.png)

In order to make things simple, we can assume that there is a simple relation between our two gaseous properties, pressure and density, which one calls the "Equation of State".  In reality, this physics/chemistry is quite complicated, but there are some situations where a simple relation holds or can be used as an empirical approximation.  One of the simplest assumptions is that the pressure only depends upon some power of the density,

![eqn of state](./images/equation_of_state.png)

where the relation then only depends upon two constants.  There are astronomical objects that obey such a simple relationship, e.g. white dwarfs, the burned out cores of  Sun-like stars that have ended their active phase of energy production and cast off most of their mass.  Such cores are so dense that the pressure is due to the refusal of the electrons to be squeezed any farther, a quantum-mechanical effect called "degeneracy".  For moderate temperatures and densities (at least by white dwarf standards), the Equation of State is a reasonably simple function of physical constants and equal to

![WD eqn of state](./images/wd_equation_of_state.png)


---

## Solving the equations

In order to derive the structure of the star or planet, we have to start at the bottom, where there is a core of very dense material, and work our way up. For every step upwards in radius, the Equation of Hydrostatic Equilibrium tells us how the pressure has to change and the Equation of State tells us what the density is at that pressure. By adding more material at a larger radius, we have changed the local gravity when we try to construct the next shell of material.

![delta M](./images/delta_M.png)

blah, blah, blah, ...

---

## Improving your simuation

- When a white dwarf has a large mass, the temperature within gets very large and the thermal motions of the electrons are nearly at the speed of light, which means that the degeneracy pressure has to be calculated differently using Einstein's Theory of Special Relativity.  This results in a different "relativistic" Equation of State

![relativistic eqn of state](./images/rel_equation_of_state.png)

How does this change affect the masses and radii of your white dwarf simulations?  The density/pressure at which there is a transition from the non-relativistic to the relativistic state can be found by setting the two equations equal to each other.  Change your equation of state so that it is non-relativistic at low densities and relativistic at high densities.

- The Equation of State for very dense cold material (by stellar standards) can be approximated as a power-law. Such conditions are appropriate in the cores of massive planets like Jupiter and Saturn.  Try to find an Equation of State that will give you the right mass and radius for Jupiter.  Apply your model to Saturn, Uranus and Neptune - how well does it work?

- What power-law equation of State will produce a reasonable model for the structure of the Sun?

