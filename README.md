# Li-ion-Battery-Fault-Analysis-Using_Deep_Learning
- Overview: [Project_Poster](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Work_images/Poster_SPARK_2024.pdf)
- Detailed Report: [Project_Report](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Project_Report_Vardan_Popli_2024.pdf)

# Project Summary
***Title: Li-ion-Battery-Fault-Analysis-Using_Deep_Learning***

In this project, I focused on the fault analysis of lithium-ion batteries using a novel deep-learning approach. Initially, I familiarized myself with the concepts of ***State of Health (SoH)***
and ***State of Charge (SoC)***, understanding what constitutes battery faults, how to measure
them, and the various types of faults. I also reviewed several research papers to build a
comprehensive knowledge base. Subsequently, I delved into the degradation mechanisms of lithium-ion batteries, identifying
the physical parameters necessary to measure these degradations. This foundational
knowledge was crucial for the next phase, where I explored various deep learning
methodologies and decided to employ a ***Long Short-Term Memory (LSTM)*** model due to its
ability to capture long-term dependencies in data. I developed and tested the LSTM model using a dataset of sodium-ion coin cells prepared in
the lab, achieving an impressive ***99% accuracy***. One challenge encountered was the lack of an
instrument in the lab to measure battery temperature. To overcome this, I designed a
temperature measurement system using an NTC thermistor, a 10K ohm resistor, and an
***Arduino UNO***. With the temperature measurement system in place, I collected data over the power cycle of
an electric vehicle (EV) and calibrated it for a single ***Li-ion cell of 18650*** configuration, as
the initial data represented an entire battery pack. I then predicted the SoH using temperature, voltage, and current data for each discharge cycle. Unlike a previous experiment by a senior, which used an Artificial Neural Network (ANN) to predict SoC without considering battery
degradation, my approach included degradation effects, providing a more accurate SoH
prediction for each discharge cycle. This project demonstrates the effectiveness of using deep learning, particularly ***LSTM models, for accurately predicting battery SoH and identifying potential faults***, thereby contributing to
safer and more efficient battery management systems in electric vehicles. **Future Reference:** Generalized model for various power cycles, Predicting SoH after set
training cycles & Doing prediction for complete pack Dynamics considering environmental
factors.

# Jupyter_Notebook
This Section Consists of Four Notebooks
- [Li_ion_Cell_EDA_and_model](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Jupyter_Notebook/Li_ion_Cell_EDA_and_model.ipynb) has LSTM model Trained on Li-ion time-series Battery Parameters (Temperature, current and Voltage) to Predict State-of-Health of the battery with Discharging Cycles
- [LSTM_Model_Using_Na+_data](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Jupyter_Notebook/LSTM_Model_Using_Na%2B_data.ipynb) has the LSTM model Trained on sodium coin cell data (Prepared and Generated in Energy Storage Laboratory, IIT ROORKEE)
- [Data_Analysis_for NASA_Battery_Dataset](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Jupyter_Notebook/Data_Analysis_for%20NASA_Battery_Dataset.ipynb) This notebook has practice EDA performed on Existing universal Dataset Prepared by NASA on Li-ion Battery 18650 cell
- [Na+_cell_EDA](https://github.com/vardanpopli/Li-ion-Battery-Fault-Analysis/blob/main/Jupyter_Notebook/Na%2B_cell_EDA.ipynb) This notebook has the EDA performed over Na+ coin cell Data using ***NMC*** composition.
