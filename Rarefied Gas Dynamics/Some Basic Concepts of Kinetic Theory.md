
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [The Velocity Distribution Function](#the-velocity-distribution-function)
- [Macroscopic Properties](#macroscopic-properties)
- [Binary Elastic Collisions of Molecules](#binary-elastic-collisions-of-molecules)
- [Collision Cross-sections and Molecule Models](#collision-cross-sections-and-molecule-models)
    - [Hard Sphere Model](#hard-sphere-model)
    - [The Inverse Power Law Model](#the-inverse-power-law-model)
    - [Maxwell Model](#maxwell-model)
    - [Variable Hard Sphere (VHS) Model](#variable-hard-sphere-vhs-model)
    - [Variable Soft Sphere (VSS) Model](#variable-soft-sphere-vss-model)
    - [Generalized Hard Sphere (GHS) Model](#generalized-hard-sphere-ghs-model)
    - [Generalized Soft Sphere (VSS) Model](#generalized-soft-sphere-vss-model)

<!-- /code_chunk_output -->

# The Velocity Distribution Function

Integrating this formula over the entire velocity space, we obtain the number of molecules in $\mathrm{d}\bm{r}\equiv\mathrm{d}x\mathrm{d}y\mathrm{d}z$, and the **number density** of the molecules in the physical space is obviously
$$ n=\int f\mathrm{d}\bm{c}$$

# Macroscopic Properties

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

# Binary Elastic Collisions of Molecules

To see the importance of binary collision we first analyze the condition under which the **ternary collisions** (three-body collisions) are rear events but the **binary collisions** prevail. The frequency of the triple collision is
$$ \left(\sigma^{1/2}/\overline{c_r}\right)\cdot(n\overline{\sigma c_r}) \approx \sigma^{3/2}n \approx d^3n \approx d^3/\delta^3 $$

where $\delta=n^{-1/3}$ is the **average molecular spacing**. It is seen, when the condition of the **dilute gas**
$$ \delta \equiv n^{-1/3} \gg d $$

is satisfied, the condition that only the binary collision is important is also satisfied.

To fully determine the collision, we need to specify the  **pre-collision velocities** $\bm{c_1}$ and $\bm{c_2}$, two **impact parameters** and the **intermolecular potential**. The two impact parameters are the distance $b$ of the projected distance between the pre-collision velocities, it is also called the **miss distance**) and the **deflection angle** $\varepsilon$ between the collision plane (in which the trajectories lie in this system of coordinates) and some reference plane.

# Collision Cross-sections and Molecule Models

The **differential collision cross-section** $\sigma$ is defined as the cross section corresponding to **unit solid angle** $\mathrm{d}\Omega$, that is,
$$ \sigma\mathrm{d}\Omega = \sigma \sin \chi \mathrm{d}\chi \mathrm{d}\varepsilon = b\mathrm{d}b\mathrm{d}\varepsilon $$

so one has
$$ \sigma = \frac{b}{\sin\chi}\left|\frac{\mathrm{d}b}{\mathrm{d}\chi}\right|$$

The **total collision section** $\sigma_T$ is obtained from the differential one through integrating over the entire solid angle
$$ \sigma_T = \int\limits_0^{4\pi} \sigma \mathrm{d}\Omega = \int\limits_o^{2\pi} \mathrm{d}\varepsilon \int \sigma\sin\chi\mathrm{d}\chi = 2\pi\int b\mathrm{d}b $$

>To find the collision cross-section $b$ is of course not to be considered as simple geometrical coordinate and integrated. *Only under certain model of the intermolecular force*, that is, when the relation between the deflection angle $\chi$ and $b$ is known, the definition of $\sigma$ and $\sigma_T$ through $b$ has meaning.

In treating practical problems of molecular motion, not only the total crosssection plays important role, but the cross-sections relevant to the
*transport properties* of the gas also play important role. These are the so called **viscosity cross-section** $\sigma_\mu$ and **diffusion cross-section** $\sigma_D$
$$ \sigma_\mu = \int\limits_0^{4\pi}\sin^2\chi\sigma\mathrm{d}\Omega = 2\pi\int\sigma\sin^3\chi\mathrm{d}\chi = 2\pi\int\sin^2\chi b\mathrm{d}b $$

$$ \sigma_D = \int\limits_0^{4\pi}(1-\cos\chi)\sigma\mathrm{d}\Omega = 2\pi\int\sigma(1-\cos\chi)\sin\chi\mathrm{d}\chi = 2\pi\int(1-\cos\chi) b\mathrm{d}b $$

Viscosity cross-section $\sigma_\mu$ appears in the expression of the viscosity $\mu$ in the transport theory of Chapman-Enskog
$$ \mu = \frac{(5/8)(\pi mkT)^{1/2}}{[m/(4kT)]^4\int\limits_0^\infty c_r^7\sigma_\mu\mathrm{exp}[-mc_r^2/(4kT)]\mathrm{d}c_r} $$

Similarly, the diffusion collision cross-section $\sigma_D$ appears in the expression of the diffusivity of binary *gas mixture* in the transport theory of Chapman-Enskog. The latter cross-section is also called **momentum transfer cross-section** $\sigma_M$.

## Hard Sphere Model

The viscosity in the hard sphere model is
$$ \mu = \frac{5}{16}(mkT/\pi)^{1/2}/d_{12}^2 $$

where $d_{12}=\frac{1}{2}(d_1+d_2)$ is the distance of the closest approach of the two molecules.

## The Inverse Power Law Model

The force and potential of the **inverse power law model** or the **repulsion point center model** is given by the following force expressions
$$ F=\kappa/r^\eta $$

Or in terms of potential
$$ \phi = \kappa/[(\eta-1)r^{\eta-1}] $$

The hard sphere model is a special case of this model with $\eta = \infty$.
The differential cross-section of this model is
$$ \sigma\mathrm{d}\Omega = b\mathrm{d}b\mathrm{d}\varepsilon = W_0\left[\frac{\kappa}{m_r c_r^2}\right]^{\frac{2}{\eta-1}}\mathrm{d}W_0\mathrm{d}\varepsilon $$

where $m_r=\frac{m_1 m_2}{m_1+m_2}$ is **reduced maas**, $W_0=b(m_r c_r^2/\kappa)^{1/(\eta-1)}$ is the dimensionless miss distance.

>When $\eta$ has finite value, the integral of the *total cross-section* diverges, but the *viscosity and diffusion collision crosssections* are convergent.

In such circumstances, it is usually necessary to make finite truncation either of miss distance $b$ or deflection angle $\chi$.

>Note, as the stipulation of $W_{0,m}$ is arbitrary, this *total cross-section* can not be used to define the collision frequency or the mean free path.

The viscosity for the inverse power law molecule is
$$ \mu = \frac{5m(RT/\pi)^{1/2}(2mRT/\kappa)^{\frac{2}{\eta-1}}}{8A_2(\eta)\Gamma\left[4-\frac{2}{(\eta-1)}\right]} $$

where
$$ A_2(\eta) = \int\limits_0^\infty\sin^2\chi W_0\mathrm{d}W_0 $$

## Maxwell Model

The special case of the inverse power law model with $\eta=5$ is called the **Maxwellian model** and it's viscosity is linearly proportional to the temperature.
$$ \mu = \frac{2kT}{3\pi A_2(5)}\left(\frac{m}{2\kappa}\right)^{1/2} $$

This is unrealistic, and thus the Maxwell molecule has significant limitations.

## Variable Hard Sphere (VHS) Model

Unfortunately, the hard sphere molecule has fixed cross-section, but the collision cross-section of real gas changes with the relative velocity (decreases with the increase of $c_r$). The difference of various molecular models manifests in the different dependence of the viscosity $\mu$ on the temperature $T$. For hard sphere, $\mu$ is proportional to $T$ in the power of `1/2`, but in real gas (for oxygen, nitrogen and air) this power isnear `0.75`.

The **VHS model** or the **Variable Hard Sphere model** stipulates that the collision cross-section is proportional to the inverse power of the relative velocity while the molecules possess isotropic scattering probability as the hard sphere.
$$ (\sigma_T/\sigma_{T,ref}) = (d/d_{ref})^2 = (c_r/c_{r,ref})^{-2\xi} = (\varepsilon_t/\varepsilon_{t,ref})^{-\xi} $$

where the reference values $\sigma_{T,ref}$, $d_{ref}$, $c_{r,ref}$ and $\varepsilon_{t,ref}$ are introduced for the total crosssection $\sigma_T$, molecular diameter $d$, relative velocity $c_r$ and relative translational energy $\varepsilon_t$, where $\sigma_{T,ref}$ and $d_{ref}$ are the values when the relative velocity is $c_{r,ref}$.

The deflection angle $\chi$, the relation of the viscosity collision cross-section $\sigma_\mu$, diffusion cross-section $\sigma_D$ with the total cross-section $\sigma_T$, is the same as the ==hard sphere model==
$$ b=d\cos(\chi/2), \quad \sigma_\mu=\frac{2}{3}\sigma_T, \quad \sigma_D=\sigma_T $$

That is, the deflection angle $\chi$ does not depend on $c_r$ explicitly. One can calculate the viscosity by writting $\sigma_T$ as $(c_r/c_{r,ref})^{-2\xi}\sigma_{T,ref}$
$$ \mu = \frac{\frac{15}{8} (\pi mk)^{1/2} (4k/m)^\xi T^{1/2+\xi}}{\Gamma(4-\xi) \sigma_{T,ref}c_{r,ref}^{2\xi}} $$

By adjusting the power $\xi$ in the definition formula, one can attain the required power $\omega$ in the dependence of viscosity on temperature
$$ \mu \propto T^\omega $$

For this one only needs to put
$$ \frac{1}{2}+\xi = \omega = \frac{1}{2}\frac{\eta+3}{\eta-1} $$

or
$$ \xi = \omega-\frac{1}{2} = \frac{2}{\eta-1} $$

with the power $\eta$ in the inverse power law.
>For the *hard sphere (HS) model* one has $\omega=1/2, \eta=\infty \text{ and } \xi=0$, for the *variable hard sphere (VHS and also the inverse power law IPL)* molecule with $\omega=0.75$, one has $\eta=9$ and $\xi=0.25$, and for the *Maxwellian molecule* one has $\omega=1, \eta=5$ and $\xi=1/2$.

>The hard sphere model with $\eta=\infty$ is the most hard molecule, and the Maxwellian molecule is the most soft among the molecular models under study.

## Variable Soft Sphere (VSS) Model

But for inverse power law molecule, the ratio of $\sigma_D$ to $\sigma_\mu$ is $A_1(\eta)/A_2(\eta)$. This results in quite large deviation from practice of the VHS model in considering *multi-component gas mixture with diffusion* playing essential role.

Koura and Matsumoto introduced the **variable soft sphere (VSS) model** and overcame this shortcoming of the VHS model. They suggest that the total cross-section (or the molecular diameter) depends on the energy during the collision as in the VHS model, but the **scattering law** of the VSS model is
$$ b=d\cos^\alpha(\chi/2) $$

where $d$ and $\alpha$ both depend on the relative energy in the collision, $\alpha$ being the power of the cosine of the deflection angle.

>As $d$ is variable and for $\alpha>1$ (it is the case for real gas) the deflection angel $\chi_{\scriptscriptstyle VSS}$ is less than the deflection angle $\chi_{\scriptscriptstyle VHS}$ of the HS and VHS model, so it is named the variable soft sphere model.

For the VSS model, it is easy to obtain
$$ \sigma_T = 2\pi \int b\mathrm{d}b = \pi d^2 $$

$$ \sigma_\mu = 2\pi\int\sin^2\chi b\mathrm{d}b = 2 \pi d^2 \int (1-\cos^2\chi)\left(\cos\frac{\chi}{2}\right)^\alpha\mathrm{d}\left(\cos\frac{\chi}{2}\right)^\alpha = S_\mu \frac{2}{3}\sigma_T $$

$$ \sigma_D = 2\pi\int(1-\cos\chi) b\mathrm{d}b = 2\pi d^2\int(1-\cos\chi)\left(\cos\frac{\chi}{2}\right)^\alpha\mathrm{d}\left(\cos\frac{\chi}{2}\right)^\alpha = S_D \sigma_T $$

where
$$ S_\mu=\frac{6\alpha}{(\alpha+1)(\alpha+2)} $$

$$ S_D=\frac{2}{\alpha+1} $$

are called **soft coefficients** of viscosity and diffusivity collision cross-sections, respectively.
Equalizing the ratio for the VSS model to the ratio for the inverse power law model
$$ \frac{\sigma_\mu}{\sigma_D} = \frac{2S_\mu}{3S_D} = \frac{A_2(\eta)}{A_1(\eta)} $$

the value of $\alpha$ is obtained
$$ \alpha = \left[\frac{A_1(\eta)}{A_2(\eta)}-\frac{1}{2}\right]^{-1} $$

The viscosity $\mu$ under the VSS model is obtained by
$$ \mu_{\scriptscriptstyle VSS} = \mu_{\scriptscriptstyle VHS}/S_\mu = \frac{5(\alpha+1)(\alpha+2)(\pi mk)^{1/2}(4k/m)^\xi T^{\frac{1}{2}+\xi}}{16\alpha\Gamma(4-\xi)\sigma_{T,ref}c_{r,ref}^{2\xi}} $$

>For all HS, VHS and VSS models there is the invariance of the relative velocity $c_r^*$ before and after collision. For HS and VHS molecules there is the result of the *isotropic distribution* of the post-collision velocity $c^*$ over all directions.

## Generalized Hard Sphere (GHS) Model

The inverse power law describes the intermolecular action as a *pure repulsion force*. For flow fields around re-entry vehicles, the temperature variation range is very large, the dependence of viscosity on the temperature can not be represented entirely by an one-exponent power law. The interaction between molecules except the short distance repulsion force *reveals the attraction character at large intermolecular distances*. A molecular model capable of reproducing **attractive-repulsive potential** is desirable.

The **generalized hard sphere (GHS)** introduced by Hassan and Hash, contains the intermolecular force that possesses both attraction and repulsion. *Its scattering law is similar with the hard sphere model*, but the relation of its total cross-section $\sigma_T$ with the relative kinetic energy $\varepsilon_t$ allows the reproduction of the attractive-repulsive potential.
$$ \sigma_T/l^2 = \Sigma\alpha_j \left(\frac{\varepsilon_t}{\varepsilon}\right)^{-\xi_j} $$

where $\varepsilon$ has the dimension of energy, $l$ has the dimension of length and is ==a parameter depending on the gas component==, $\varepsilon_t=\frac{1}{2}m_r c_r^2$ as before.

The scattering law is taken the same as the hard sphere, i.e.
$$ b=d\cos(\chi/2) \quad \text{or} \quad \sigma_\mu=\frac{2}{3}\sigma_T $$

One can also obtain the viscosity
$$ \mu = \frac{\frac{15}{8} (\pi mkT)^{1/2}/l^2}{\Sigma\alpha_j \Gamma(4-\xi_j) (kT/\varepsilon)^{-\xi_j}} $$

If the two-term expression is used, then
$$ \mu = \frac{\mu_0}{1+ST^{\xi_1-\xi_2}} $$

$$ \mu_0 = \frac{15}{8}\frac{(\pi mkT)^{1/2} (kT/\varepsilon)^{\xi_1}}{\alpha_1 \Gamma(4-\xi_1) l^2}, \quad S = \frac{\alpha_2}{\alpha_1}\frac{\Gamma(4-\xi_2)}{\Gamma(4-\xi_1)}\left(\frac{k}{\varepsilon}\right)^{\xi_1-\xi_2} $$

Let $\xi_1=1, \xi_2=0$, the **viscosity law of Sutherland** is obtained.
For the **Lennard-Jones interaction potential**
$$ F=\frac{\kappa_{12}}{r^\eta}-\frac{\kappa_{12}'}{r^{\eta'}}, \quad \eta>\eta'$$

Chapman and Cowing gives the following expression of the viscosity for the Lennard-Jones interaction potential
$$ \mu=\mu_{\scriptscriptstyle IPL}/\left(1+ST^{-\frac{\eta-\eta'}{\eta-1}}\right) $$

where $\mu_{\scriptscriptstyle IPL}$ is the expression of the viscosity under iiverse power law. Compared with the two-term expression, it yields
$$ \xi_1=\frac{2}{\eta-1}, \quad \xi_2=\frac{2-\eta'+\eta}{\eta-1} $$

For the Lennard-Jones 6-12 $(\eta = 13, \eta' =7)$ model, one has $\xi_1=1/6, \xi_2=2/3$.

## Generalized Soft Sphere (VSS) Model

The simultaneous adoption of the GHS dependence of $\sigma_T$ on $\varepsilon_t$ and the VSS molecular scattering law $b=d\cos^\alpha(\chi/2)$ which naturally lead to the **generalized soft sphere (GSS) model**.

>The GSS model is of meaning especially for the case of low temperature and polar mofecules. e.g. The **Stockmayer potential**, which takes into account the electrostatic interaction between polar molecules.