
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [The velocity distribution function](#the-velocity-distribution-function)
- [Macroscopic properties](#macroscopic-properties)
- [Binary elastic collisions of molecules](#binary-elastic-collisions-of-molecules)

<!-- /code_chunk_output -->

# The velocity distribution function

Integrating this formula over the entire velocity space, we obtain the number of molecules in $\mathrm{d}\bm{r}\equiv\mathrm{d}x\mathrm{d}y\mathrm{d}z$, and the **number density** of the molecules in the physical space is obviously
$$ n=\int f\mathrm{d}\bm{c}$$

# Macroscopic properties

The **density** $\rho$ of the gas in the physical space is obviously
$$ \rho = m\int\limits_{-\infty}^{\infty}\int\limits_{-\infty}^{\infty}\int\limits_{-\infty}^{\infty}f\mathrm{d}u\mathrm{d}v\mathrm{d}w \equiv m\int f\mathrm{d}\bm{c} \equiv mn $$

where $m$ is the mass of the molecule.
The **mean molecular velocity** $\overline{\bm{c}}$ is the **macroscopic stream velocity** of the gas, or the **mean velocity**, or the **mass velocity** of the gas.
$$ \overline{\bm{c}} = \frac{1}{n}\int\bm{c}f\mathrm{d}\bm{c} $$

Generally, if $Q(\bm{c})$ is an arbitrary function of the molecular velocity, its **mean value** $\overline{Q}$ in the gas is defined as
$$ \overline{Q} = \frac{1}{n}\int Qf\mathrm{d}\bm{c}$$

$Q$ may represent scalar, vector or tensor.
The velocity $\bm{c}-\overline{\bm{c}}$ of a molecule relative to the macroscopic stream velocity is called the **thermal velocity**, or **peculiar velocity**, some times is also called the **random velocity** of the molecule and is denoted by $\bm{c'}$
$$ \bm{c'}=\bm{c}-\overline{\bm{c}} $$

We obtain the **flux** of $Q$, i.e. the quantity of $Q$ carried by the molecules crossing an area *per unit area per unit time*
$$ n\overline{Q\bm{c}}\cdot\bm{l} = n\overline{Q\bm{c\cdot l}} = \int Q \bm{c\cdot l} f \mathrm{d}\bm{c}$$

$\bm{l}$ is the unit normal vector of this area element. Above equation is a **total flux**, it includes the fluxes of molecules crossing the area in the positive $\bm{l}$ direction and in the opposite $\bm{l}$ direction.
Some times the flux crossing $\mathrm{d}S$ only in one direction is needed to be known. For example the flux of $Q$ in the positive $\bm{l}$ direction is
$$ n\overline{(Q\bm{c\cdot l})}_{\bm{c\cdot l}>0} $$

We can define $n\overline{Q\bm{c}}$ as the **flux vector** of quantity $Q$
$$ n\overline{Q\bm{c}} $$

Let $ Q=m\bm{c'}$, we attain the expression of the *momentum transport* caused by the thermal motion. The expression so obtained is a tensor with nine components, and is called the **pressure tensor** $\bm{P}$
$$ \bm{P} = \int m\bm{c'}\bm{c'}f\mathrm{d}\bm{c} = nm\overline{\bm{c'}\bm{c'}} = \rho\overline{\bm{c'}\bm{c'}} $$

At an arbitrary point inside the gas, the **pressure (pressure flux)** $\bm{p}_l$ acting on $\mathrm{d}S$ and pointing in the positive direction of the surface is the flux of molecular momsntum me across this surface along the positive direction (per unit time, per unit area).
$$ \bm{p}_l = \int m\bm{c'}\bm{c'\cdot l} f\mathrm{d}\bm{c} = \rho\overline{\bm{c'c'}}\cdot \bm{l} = \bm{P\cdot l} $$

As the direction of the stress exerted by the gas on the surface is opposite to the direction of the momentum flux, we define the **viscous stress tensor** $ \bm{T} \equiv \tau_{ij}$ as the negative of the pressure tensor with the **static pressure** $p$ subtracted from the normal components
$$ \bm{T} \equiv \tau_{ij} = -(\rho\overline{c_i'c_j'}-\delta_{ij}p) $$

or
$$ P_{ij} = p\delta_{ij}-\tau_{ij} $$

where $p$ is the **static pressure**, defined as the average of the three normal components of the pressure tensor
$$ p = \frac{1}{3}\rho\overline{u'^2+v'^2+w'^2} = \frac{1}{3}\rho\overline{c'^2} $$

To obtain the expression of the **heat flux** $\bm{q}$, we start again from $n\overline{Q\bm{c'}}$, this time one lets $ Q = (1/2)mc'^2+\varepsilon_{in}$, where $\varepsilon_{in}$ is the internal (vibrational or rotational) energy related to one molecule, then
$$ \bm{q} = \int (\frac{1}{2}mc'^2+\varepsilon_{in})\bm{c'}f\mathrm{d}\bm{c} = \frac{1}{2}\rho\overline{c'^2\bm{c'}}+n\overline{\varepsilon_{in}\bm{c'}} $$

One can also obtains the expression of the **specific translational energy** and introduce the **translational kinetic temperature**
$$ \frac{3}{2}\frac{k}{m}T_{tr} = e_{tr} = \frac{1}{2}\overline{c'^2} = \frac{1}{2}(\overline{u'^2}+\overline{v'^2}+\overline{w'^2}) = \frac{3}{2}\frac{p}{\rho} $$

One can define separately the translational kinetic temperatures for three velocity components
$$ \frac{k}{m}(T_{tr})_x = \overline{u'^2}, \quad \frac{k}{m}(T_{tr})_y = \overline{v'^2}, \quad \frac{k}{m}(T_{tr})_z = \overline{w'^2}$$

>The above discussions have been proceeded without any assumptions about the state of the gas, that is, they are applicable both for the *equilibrium* and *non-equilibrium* states.

In the gas of *monatomic molecules* $T_{tr}$ can be defined as the temperature of the gas. However, The *diatomic and polyatomic molecules* have rotational and vibrational energy modes and the corresponding internal degrees of freedom.
According to the number $\zeta$ of degrees of freedom of internal energy mode, the **internal kinetic temperature** $T_{int}$ of this internal energy mode can be defined as
$$ \frac{\zeta}{2}\frac{k}{m}T_{int} = e_{int} = e_r+e_v $$

The **energy equipartition principle** implies the equality of the translational and internal temperature of the gas in *equilibrium* state. In the *non-equilibrium* gas, an **overall kinetic temperature** $T_{ov}$ can be defined
$$ T_{ov} = (3T_{tr}+\zeta T_{int})/(3+\zeta) $$

# Binary elastic collisions of molecules

To see the importance of binary collision we first analyze the condition under which the **ternary collisions** (three-body collisions) are rear events but the **binary collisions** prevail. The frequency of the triple collision is
$$ \left(\sigma^{1/2}/\overline{c_r}\right)\cdot(n\overline{\sigma c_r}) \approx \sigma^{3/2}n \approx d^3n \approx d^3/\delta^3 $$

where $\delta=n^{-1/3}$ is the **average molecular spacing**. It is seen, when the condition of the **dilute gas**
$$ \delta \equiv n^{-1/3} \gg d $$

is satisfied, the condition that only the binary collision is important is also satisfied.

To fully determine the collision, we need to specify the  **pre-collision velocities** $\bm{c_1}$ and $\bm{c_2}$, two **impact parameters** and the **intermolecular potential**. The two impact parameters are the distance $b$ of the projected distance between the pre-collision velocities, it is also called the **miss distance**) and the **angle** $\varepsilon$ between the collision plane (in which the trajectories lie in this system of coordinates) and some reference plane.