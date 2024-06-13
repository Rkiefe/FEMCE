# FEMCE (Finite Element Magnetocaloric Effect)
A free to use 3D software for the magnetocaloric effect calculation. Accepts STL files of refrigerant designs or you can design your own simple shapes with the built-in model maker.

## Functionality
FEMCE is made for the evaluation of the magnetocaloric effect on real-world 3D shaped refrigerants with possibly non-linear magnetic properties. For example: gadolinium sheets distanced a few mm from each other.

It allows the user to import 3D designs built with external tools such as Blender (by STL files), and calculate both the heterogeneous magnetic field and magnetocaloric effect for the thermodynamic properties provided by the user (specific heat and magnetization).

It outputs the effective, maximum and minimum \( \Delta T \) and \( \Delta S \) as well as its magnetization and other important results.

## Method
FEMCE, as the name implies, uses the finite element method to solve a non-linear magnetostatic equation to calculate the 3D magnetic field \(H\), which is considered constant on each element of the mesh. The non-linearity is approached through a variation on the Piccard iteration method.
