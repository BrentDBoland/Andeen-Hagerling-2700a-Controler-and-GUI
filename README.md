# Install
This .vi was created using LabVIEW2017 and may not be compatible with other versions. Add the Andeen-Hagerling folder to your LabVIEW instr.lib folder to install the driver library before opening Andeen-Hagerling-2700a-Controler-and-GUI.vi
# File settings
<img width="522" height="203" alt="image" src="https://github.com/user-attachments/assets/e664554c-91e8-4eb9-bbcb-1a3c7ffd41f3" />

choose a save folder for your data. You will choose a label for your sample and the date will be appended to the label to create the file name. Hear you can also specify externally measured temperature, relative humidity, and pressure to be included in the meta data.
# Bridge settings
<img width="236" height="282" alt="image" src="https://github.com/user-attachments/assets/3cacd792-33ea-40fa-936a-edc25e774559" />

These values correspond to the settings of the AH2700A. These settings will be saved as meta data. For more information refer to the AH2700A manual.
# Frequency sweep settings
<img width="506" height="172" alt="image" src="https://github.com/user-attachments/assets/08967bbb-ff91-4ff4-9077-a50d27355db2" />

There are 3 frequency sweep options standard, custom, and 600+ Hz. Standard is a pseudo logarithmic sweep from 50 to 20,000 Hz with 27 total frequencies. Custom allows you to create your own list of desired frequencies. 600+ Hz is the same as standard, but skips all frequencies below 600 for faster data acquisition sweeping a total 16 frequencies. You can choose to repeat frequency measurements for increased accuracy under Freq Reps. If desired, you can also set a delay between measurements. Data collection can be randomized in two ways. Rand Freq chooses a frequency at random and then takes all repetitions before moving on to a new random frequency until all desired frequences have been measured. Rand Meas chooses a frequency at random and then measures only one repetition before choosing a new frequency at random until all frequency repetitions have been measured.
# Display
<img width="1069" height="947" alt="image" src="https://github.com/user-attachments/assets/ab0bcdad-ee08-4735-8a17-eb72d78dc053" />
The GUI will plot the measured capacitance and the loss measurement (assumed to be tan d in labeling, but will be whatever unit you choose in the unit setting) vs frequency and update as measurements are taken. It will also display any error messages received, your measurement progress, and the most recent measurement.
