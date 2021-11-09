Further development of the density based solution algorithm for computational modelling of high energy multiphase flows blastfoam 3.5 by Usman Rana (PhD. candidate) and Dr.Thomas Abadie from Matar Fluid Group of Prof. Omar Matar at Imperial College London.


Current status: 

bird-carreau viscosity model: 

strain rate can be used in the mu function in blastfoam/src/thermodynamicModels/specie/transportModels/const/constTransport.H.

strain rate is getting updated added after adding to encode() in compressibleSystem libraries.


Following changes have been made:

-U (velocity) and sr (strainRate) added to all thermo libraries in blastfoam/src/thermodynamicModels/basic 

-U (velocity) and sr (strainRate) added to all thermo libraries in blastfoam/src/thermodynamicModels/derived

- sr added as a primitive variable (like U, rho, p) to the compressibleSystem libraries in blastfoam/src/compressibleSystem/multiphaseCompressibleSystem


- sr added as a primitive variable (like U, rho, p) to the compressibleSystem libraries in blastfoam/src/compressibleSystem/phaseCompressibleSystem

- sr added as a primitive variable (like U, rho, p) to the compressibleSystem libraries in blastfoam/src/compressibleSystem/singlePhaseCompressibleSystem

- sr added as a primitive variable (like U, rho, p) to the compressibleSystem libraries in blastfoam/src/compressibleSystem/twoPhaseCompressibleSystem

-sr added as a primitive variable (like U, rho, p) to the update function in the fluxSchemes files in blastfoam/fluxSchemes/fluxScheme
