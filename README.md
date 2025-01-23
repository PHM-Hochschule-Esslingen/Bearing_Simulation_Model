# Description of the Simulation Model
[Mauthe, Hagmeyer, and Zeiler (2025)](#Citation) propose this simulation model for generating representative run-to-failure data of rolling bearings. It is designed to address challenges in data-driven diagnostic and prognostic methods in the context of Prognostics and Health Management (PHM), such as unbalanced or limited data availability. The model consists of three modular components: the life and fault modeling, the degradation progression simulation, and the vibration signal generation. Each module incorporates random processes to reproduce real-world variations, such as differences in bearing lifetimes and degradation progressions under similar operating conditions. The model simulates vibration signals throughout a bearing's life, reflecting both operating and degradation conditions. As such, the versatile model enables its users to create synthetic data sets of rolling bearings tailored to specific scenarios. Further information can be found in ([Mauthe, Hagmeyer, and Zeiler, 2025](#Citation)).

# Utilization of the Simulation Model
The simulation model is implemented in MATLAB (for details, see [Specifications](#Specifications)). All files and functions required for using the model are contained in the “Simulation_Model” ZIP file. All files and functions must be located in the same folder when using the model. For doing so, only the following two files must be considered:
### Main_User.m
This script must be run in MATLAB in order to carry out a simulation. Among other things, it can be used to specify whether the simulated data should be saved or not. In the case of data saving, a folder is automatically created in the current folder during the simulation in which the results are stored. The name of the folder can be defined by the user in the Main_User.m script.
### Simulation_Parameters.xlsx
The input information required for the simulation must be defined by the user in the “Simulations_Parameters.xlsx” spreadsheet file. The file name can be changed, but the change must then also be made in Main_User.m. This spreadsheet serves as the basis for the simulation. It is very important to ensure that the **column names in the first row are not changed!** The corresponding variables in the simulation model are parameterized based on these names. The file already contains examples of values in the corresponding columns, which are intended to provide guidance and assistance. A description of the meaning of the respective parameter or the individual columns can be found in “README_Parameterization.pdf”. For a further understanding regarding the parameters, the corresponding paper, _Holistic Simulation Model of the Temporal Degradation of Rolling Bearings_ by [Mauthe, Hagmeyer, and Zeiler (2025)](#Citation), should be read. This paper also describes the structure and theoretical background of the simulation model.

## Specifications
To use the model, at least MATLAB version R2022a or higher is required. Additionally, the following toolboxes must be installed:
+ Signal Processing Toolbox
+ Statistics and Machine Learning Toolbox
+ Communications Toolbox

Currently, use is limited to the Windows OS. The authors are working on the option of using the simulation model in Linux.

# License
Creative Commons Attribution 4.0 International License (CC BY 4.0)

# Citation
Use the following citation when working with the model and using the data generated with it: Mauthe, F.; Hagmeyer, S.; Zeiler, P. (2025). Holistic simulation model of the temporal degradation of rolling bearings. In E. B. Abrahamsen, T. Aven, F. Bouder, R. Flage, and M. Yloenen (Eds.), Proceedings of the 35nd European Safety and Reliability Conference (Submitted). Research Publishing.
