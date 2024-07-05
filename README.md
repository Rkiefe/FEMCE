# FEMCE (Finite Element Magnetocaloric Effect)
A public 3D software for the magnetocaloric effect calculation. Accepts STL files of refrigerant designs or you can design your own simple shapes with the built-in model maker. **Important** It requires the freely available matlab runtime 24.1 (R2024a - https://www.mathworks.com/products/compiler/matlab-runtime.html).

## Functionality
FEMCE main proficiency is to calculate the magnetocaloric effect on real-world 3D shaped refrigerants with non-linear magnetic properties. For example: gadolinium sheets distanced a few mm from each other.

![femce_gui](https://github.com/Rkiefe/FEMCE/assets/122529294/5c5cd6bf-ac66-4d75-abf9-631bec930e26)

FEMCE allows the user to import 3D designs built with external tools such as Blender (by STL files), and calculate both the heterogeneous magnetic field and magnetocaloric effect for the thermodynamic properties provided by the user (magnetization and specific heat or temperature change as a function of field and temperature).

It outputs the effective, maximum and minimum $\Delta T$ and $\Delta S$ as well as its magnetization and other important results.

## Method
FEMCE, as the name implies, uses the finite element method to solve a non-linear magnetostatic equation to calculate the 3D magnetic field $H$, which is considered constant on each element of the mesh. The non-linearity of this magnetostatics problem is approached through a variation on the Piccard iteration method.
