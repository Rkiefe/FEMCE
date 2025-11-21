# FEMCE (Finite Element Magnetocaloric Effect)

Magnetic refrigerant designs (packed beds, channeled structures, etc) impact the performance of magnetic cooling technology in multiple fronts - heat transfer, pressure drop, self demagnetizing effects, machinability, etc. FEMCE streamlines this optimization process, providing a user-friendly, free to use, purpose-built 3D simulation software for magnetocalorics.

If you use FEMCE **please cite its article**: R. Kiefe, J.S. Amaral "FEMCE - A 3D finite element simulation tool for magnetic refrigerants" International Journal of Refrigeration available online https://doi.org/10.1016/j.ijrefrig.2025.02.017

## Features
- State-of-the-art numerical methods for maximum performance and stability (compatible with first-order phase transitions)
- Import any 3D model and make it simulation-ready with the press of a button (.stl files)
- Simplified mesh generation (set a target element size, get an optimized, locally refined tetrahedral mesh)
- Import all of the thermomagnetic data with a single button
- Freely available. No fees, no subscriptions

## Outputs
FEMCE main proficiency is to calculate the heterogeneous magnetocaloric effect (local temperature and entropy change) on real-world 3D refrigerants with non-linear magnetic properties

![Screenshot 2024-11-12 154804](https://github.com/user-attachments/assets/0a364bc3-1423-40c8-8077-04721b710a65)


FEMCE outputs the effective, maximum and minimum $\Delta T$ and $\Delta S$ as well as its local and volume-average magnetization, heat absorbed, etc.

## Method
FEMCE, as the name implies, uses the finite element method to solve a non-linear magnetostatic equation to calculate the 3D magnetic field $H$, following the so-called total magnetostatic scalar potential formulation. The non-linearity of this magnetostatic problem is handled by a careful combination of the state-of-the-art Newton-Raphson and Picard iteration methods since version 1.2.* .

## More
FEMCE can do much more when not limited by a user-interface (GUI). Additional functionalities unlocked by the source code:
- Set a temperature gradient on the refrigerant, instead of a uniform temperature
- Handle magnetocrystalline anisotropic materials
- Combine materials and refrigerants in the same simulation (add iron, magnets, multiple refrigerant compositions, etc)

For this additional features, please contact rodrigokiefe@ua.pt or jamaral@ua.pt