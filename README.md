# Advanced-Memristor-Modeling
A unified LTSpice memristor library containing the main commonly used existing standard models and several modified by Prof. V. Mladenov models. The proposed models are available for simulations of memristor circuits in LTSpise in the time domain. They could be adapted for operation in PSpice or other SPICE environments. The considered models could be tested and if needed for analysis of different memristors their parameters could be changed by the users. LTSpice is a free and user-friendly software for simulation of electronic schemes. It has a good convergence. In the near future the proposed memristor library will be expanded by new memristor models.
General information. The memristors are two-terminal nonlinear passive elements with memory effect - after turning the power sources off they retain its resistance. Their state is changing by external voltage or current signal with appropriate amplitude and frequency. In the present library the presented models are related basically to transition metal oxide-based memristors - titanium dioxide, hafnium dioxide, tantalum oxide. The memristors are investigated intensively in the recent years for their potential applications in memory circuits, reconfigurable devices, neural networks and others.
# 1. Modeling of memristors in LTSpise environment
To test the proposed models and to make and analyze memristor circuits the readers must use LTSpice software. This software could be downloaded and installed using the following link: https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html#
# 2. Information about downloading and using the memristor library models
After downloading the .zip file, unzip it and keep the obtained folder. All the proposed models are in this folder. If you make any changes of the parameters, keep the files in the same directory, the changes will be automatically considered when you apply the models in existing circuits.
# 3. LTSpice codes and creating library models
Open the unzipped folder and the model that you want to apply. Then right click on the file, select "Open with LTSpice". Then select by the mouse the abbreviation of the model in the opened file, for example A1, then right click and select "Create part". The created symbol appears with its three electrodes. The electrode Y could be connected to additional high-valued resistor (for example 1GOhm) and the next terminal of the resistor - to the ground. The others two terminals have to be connected to the respective nodes in the created circuit.
# 4. Application in memristor circuits
The generated memristor model could be inserted in a new circuit or in an existing one. For this purpose, click "Place part" in LTSpice and place the memristor by left mouse button click, or open the library "Auto generated" and select it, then press Enter. According to the manufacturing tolerances, the physical parameters and other factors changes of the memristor model parameters could be applied. For this purpose the reader must open the respective text file containing the LTSpice model, to change the memristor parameters in the sections .param, and the save the file. The next time you start the memristor model in LTSpice environment the alterations made will be automatically adressed to the respective schematic element of the considered memristor. There is no need to create the analyzed scheme again.
# 5. Description of the models
The existing standard LTSpice models are abbreviated as follows: K1 (Strukov's model), K2 (Joglekar,s model), K3 (Biolek's model), K4 (Boundary condition based model), K5 (Lehtonen-Laiho model). These models are for titanium dioxide memristors. For hafnium dioxide memristor models are valid the next 2 models: K6 (model with a simple window function), K7 (a model with highly nonlinear window function). The first 5 modified models for titanium dioxide memristors are: A1 (nonlinear drift modified model of a titanium dioxide memristor with a voltage-dependent Joglekar,s window function), A2 (nonlinear drift modified model of a titanium dioxide memristor with a modified Biolek window with additional sinusoidal component), A3 (nonlinear drift modified model of a titanium dioxide memristor with a modified Biolek window with a Voltage-Dependent Variable Exponent), A4 (nonlinear drift modified model of a titanium dioxide memristor with a modified Biolek-Joglekar window with a Voltage-Dependent Exponent), A5 (nonlinear drift modified Lehtonen-Laiho library model of a titanium dioxide memristor with a modified Biolek window and a voltage-dependent exponent), A6 (modified nonlinear drift Lehtonen-Laiho library model of a hafnium dioxide memristor with a modified Biolek window with additional sinusoidal component), A7 (modified nonlinear drift Lehtonen-Laiho library model of a hafnium dioxide memristor with a modified Biolek window with a voltage dependent exponent), A8 (modified nonlinear drift Lehtonen-Laiho library model of a hafnium dioxide memristor with a modified Joglekar window with additional sinusoidal component). Tantalum oxide memristors are available: K8 and K9 (standard models) and A9, A10 (modified models).
# 6. Advantages and drawbacks of the considered memristor models
The proposed modified memristor models A1 - A8 have applied a dependence between the nonlinear ionic dopant drift velocity and the applied voltage and additional sinusoidal component for increasing the models' nonlinearity. The models A9 and A10 are simplified with respect to the corresponding original tantalum oxide memristor models. Detailed information about the memristor library models is included in the section "Properties" in the respective codes.
# Citation
When the reader use a given memristor model from the respective library, please cite the original sources presented in the end of the respective code.
