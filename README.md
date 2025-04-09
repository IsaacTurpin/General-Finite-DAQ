# General-Finite-DAQ
## Purpose
This LabVIEW 2021 application collects finite data from multiple channels on an NI DAQ device and displays the data on a graph, offering the ability to save the acquired data to a ".csv", ."txt", or ".tdms" file. This application also offers basic anaylsis of the data, calculating the mean average of all channels and the mean of each individual channel. On top of this, the program also features the ability to read data from an existing file and displays it on the graph. To ensure no data is lost, this application automatically saves data to a binary recovery file, storing the data from the last acquisition and displaying it on the graph. This program is set up to acquire analog input voltage, n samples, n channels.

## How to use
* **Configure Data Acquisition** - Select this button to choose your DAQ device and channels, the number of samples you want to collect, your desired sample rate, and your minimum and maximum voltage values for your device, then press ok. These settings are saved to a configuration file so the application is ready for you to reuse it without having to change everything again if you don't want to. When selecting your device and channels,  enter "DeviceName/ai0" for 1 channel (channel 0 in this case), "DeviceName/ai0:3" for multiple channels (channels 0 to 3 in this case), or "DeviceName/ai0, DeviceName/ai4" for specific channels (channels 0 and 4 in this case).
* **Acquire Data** - Press this button to acquire your data from the configuration settings you selected. This will be displayed on the graph.
* **Save to File** - Use the 'File Type' drop down to select either a ".csv", ."txt", or ".tdms" file, tick the 'Open File Location' checkbox to open the file location when saved or leave it unchecked to not. Then press the 'Save to File' button to save your acquired data to a file.
* **Read Data File** - Press this button to select a file to read data from, this data will be displayed on the graph.
* **Clear Graph** - Press this button to reset the data and clear the graph.
* **Reset Settings** - Press this button to reset the settings of the application.
* **Copy Graph Image** - Press this button to copy the graph image to your clipboard.
* **Copy Graph Data** - Press this button to copy the graph data to your clipboard.
