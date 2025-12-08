# Studied Systems

This directory contains input files for molecular dynamics simulations of an equimolar mixture of $\mathrm{[Li][NTf_2]}$ and triglyme (G3), as well as a system that includes an additional equimolar amount of water. All simulations were performed using **GROMACS 2019.6**.

Simulation parameters that differ from GROMACS defaults are provided in the corresponding `SIMXX.mdp` files. For a complete list of parameters used during production runs, see `sim1out.mdp`. The initial configurations are stored in `START.gro`, and the associated force-field definitions can be found in `topol.top`. Naming conventions follow those outlined in the *GROMACS 2019.6 manual*.

The systems are labeled according to the molar ratios of their components. The folders [1_1_0](1_1_0/) and [1_1_1](1_1_1/) correspond to mixtures of $\mathrm{[Li][NTf_2]}$:G3:$\mathrm{H_2O}$ with ratios 1:1:0 and 1:1:1, respectively.

Within each system folder:

- **[sim_303K/](1_1_1/sim_303K/)** contains the input files for production runs performed in cubic simulation boxes at 303 K.
- **[orthoboxy_303K/](1_1_1/orthoboxy_303K/)** contains input files for simulations at 303 K using the *OrthoBoXY* method, employing an orthorhombic unit cell with  
  \[
  L_z/L_x = L_z/L_y \approx 2.7933596497.
  \]

Other simulations follow the same directory structure and naming logic.
