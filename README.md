# FEMCE (Finite Element Magnetocaloric Effect)
A public 3D software for the magnetocaloric effect calculation. Accepts STL files of refrigerant designs or you can design your own simple shapes with the built-in model maker.

## Functionality
FEMCE main proficiency is to calculate the magnetocaloric effect on real-world 3D shaped refrigerants with non-linear magnetic properties. For example: gadolinium sheets distanced a few mm from each other.

![femce_gui](https://github.com/user-attachments/assets/ea1554dc-990e-4203-a79e-0b52a8ffce7e)

FEMCE allows the user to import 3D designs built with external tools such as Blender (by STL files), and calculate both the heterogeneous magnetic field and magnetocaloric effect for the thermodynamic properties provided by the user (magnetization and specific heat or temperature change as a function of field and temperature).

It outputs the effective, maximum and minimum $\Delta T$ and $\Delta S$ as well as its magnetization and other important results.

## Method
FEMCE, as the name implies, uses the finite element method to solve a non-linear magnetostatic equation to calculate the 3D magnetic field $H$, which is considered constant on each element of the mesh. The non-linearity of this magnetostatics problem is approached through a variation on the Piccard iteration method.
