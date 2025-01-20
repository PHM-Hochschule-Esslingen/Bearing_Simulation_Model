# Description of the Simulation Model
This simulation model is proposed by X and Y for generating representative run-to-failure data, focusing on rolling bearings. It is designed to address challenges in data-driven diagnostic and prognostic methods in the context of Prognostics and Health Management (PHM), such as unbalanced or limited data availability, often encountered in industrial settings. The model consists of three modular components: life-load modeling, degradation progression simulation, and vibration signal generation. Each module incorporates random processes to mimic real-world variations, such as differences in bearing lifetimes and degradation paths under similar operating conditions. The model simulates vibration signals throughout a bearing's lifecycle, reflecting both operating and degradation conditions. This versatile model supports creating synthetic data sets tailored to specific scenarios, facilitating research in PHM. Further information can be found in [Mauthe, Hagmeyer, and Zeiler (2025)](#Citation).

# Utilization and Handling of the Simulation Model
The simulation model is implemented in MATLAB. To use the model, at least version MATLAB R2022a or later is required. All files and functions required for using the model are contained in the “Simulation_Model” ZIP file. This must be downloaded and unzipped. All files and functions must then be located in the same folder that is selected in MATLAB. For the use of the model, only the following two files must be considered:
### Main_User.m
This script must be run in Matlab in order to carry out a simulation. Among other things, it can be used to specify whether the simulated data should be saved or not. In the case of saving, a folder is automatically created in the current folder during the simulation in which the results are saved. The name of the folder can be defined by the user in the Main_User.m script. The input information required for the simulation must be defined by the user in the “Simulations_Parameters.xlsx” spreadsheet file. The file name can be changed, as it can also be changed in Main_User.m. All other MATLAB files have been converted into so-called p-files and are therefore read-only and cannot be changed by the user.
### Simulation_Parameters.xlsx
This spreadsheet serves as the basis for the simulation. It is therefore very important to ensure that the **column names in the first row are not changed!** The corresponding variables in the simulation model are parameterized based on these names. The file “Simulation_Parameters.xlsx” already contains examples of values in the corresponding columns, which are intended to provide guidance and assistance. A detailed description of the meaning of the respective parameter or the individual columns can be found in "README.pdf". In addition, the corresponding paper _Generic Model for Holistic Simulation of the Temporal Degradation of Rolling Bearings_ by [Mauthe, Hagmeyer, and Zeiler (2025)](#Citation) should be read. This paper describes the structure and theoretical background of the simulation model.

## Specifications
To use the model, at least version MATLAB R2022a or later is required. The following toolboxes must be installed: …

Currently, use is still limited to the Windows OS. The authors are working on the option of using the simulation model in Linux.

# Licenses
...

# Citation
Use the following citation when working with the model and using the data generated with it: Mauthe, F., S. Hagmeyer, and P. Zeiler (2025). Generic model for holistic simulation of the temporal degradation of rolling bearings. In E. B. Abrahamsen, T. Aven, F. Bouder, R. Flage, and M. Yloenen (Eds.), Proceedings of the 35nd European Safety and Reliability Conference (Submitted). Research Publishing.

