# Infant8
Description:
A new Infant approach searches for the global minimum chemical structures (complexes, large biomolecular systems) along vibrational modes calculating the energies of intramolecular (MM3 force field) and intermolecular (Model of Effective Radii of Atoms (MERA)) interactions with the possibility of fixing structural fragments
The program is the serious modification of MM3 codes developed by Jay William Ponder. Dr. Maria Grishina and Dr. Vladimir Potemkin included new algorithms for searching for a global minimum of energy, calculating the energies of intermolecular interactions calculated using the Model of Effective Atomic Radii (MERA), and allowed fixing structural fragments that should not change during optimization. Infant allows searching for a global minimum of the structure along vibrational modes using Cartesian coordinates (useful for modeling a structure that includes 2 or more molecules to optimize their position relative to each other and conformational adjustment), using torsional modes (useful for determining the most stable conformational state) and a local minimum. The choice of the type of calculations is available in the line "Local Search Type - Cartesian, Torstional and None (C T or [N])". For a Cartesian search, type "C"; for a torsional search, type - "T", for a local minimum, type "N" or just press enter.
Initial structure must include all atoms including hydrogens. Infant is mostly available for the chemical systems with atoms-organogens and halogens.

How to start computations:
1) Copy mm3m.prm in the C:\pva\crypt\mech\mm3m.prm 
2) In the command line, type the program name (infant8.exe) and press enter. Then write the name of the hin (HyperChem) file with the initial structure that needs to be optimized. The initial structure can be a large molecular system (1 or more molecules) with a total number of atoms up to 10,000, with selected structural fragments, the geometry of which should not change during optimization.
3) Then select "Local Search Type - Cartesian, Torstional and None (C T or [N])" and press enter to start computations.

The result file is the .002 file which has the hin file format. All other files .999, .000, .500, ... can be deleted. Rename the .002 file to .hin and open this file with HyperChem or any other application that supports the hin format.
