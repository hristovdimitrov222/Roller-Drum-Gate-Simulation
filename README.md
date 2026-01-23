# OpenFOAM CFD simulation of flow under roller drum gate
The code provided here is supplementary to the paper Berghammer, L.M., & Dimitrov, H. (2026). Influence of a jet guiding structure on flow under a roller drum gate – Comparison of flow measurements and numerical simulations. *11th IAHR International Symposium on Hydraulic Structures*, Chengdu, China. ISSN: ..., DOI: https://doi.org/[DOI] . The code is for the Volume-of-Fluid solver "interfoam" of OpenFOAM. The meshes and simulation setups are separated to "with extension" and "without extension", referring to with and without jet-guiding structure. For "without extension" there are subfolders to check the prefilled setup and the filling one. 

The code can be altered and shared freely. 
 
# How to use
Download the desired cases for testing from the [inter](inter) folder. Run the following commands:

```
decomposePar
mpirun -np 5 interFoam -parallel
reconstructPar
rm -r processor*
```
Observe the results in a post-processing software.

For further understanding of the boundary conditions and how to set them up, please refer to Thorenz, C. (2024): 'Boundary Conditions for Hydraulic Structures Modelling with OpenFOAM', 10th International Symposium on Hydraulic Structures, Zürich. ISSN 0374-0056 , DOI: https://doi.org/[10.3929/ethz-b-000675949] or [HydBCsForOF](https://github.com/baw-de/HydBCsForOF/tree/v2412).

# Development
**OpenFOAM CFD simulation of flow under roller drum gate** is developed by the [Technical University of Munich](https://www.tum.de/en/).

# License
**OpenFOAM CFD simulation of flow under roller drum gate** is distributed by the [Technical University of Munich](https://www.tum.de/en/) and is freely available and open source, licensed under the [GNU General Public License 3](https://www.gnu.org/licenses/gpl-3.0.html).
See [License](LICENSE) for details.
