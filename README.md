# sipm-array
Schematics and layouts for SiPM arrays

# tia-s14160-x4
This contains schematics and PCB layouts for a 4 channel SiPM detection board used for parallel laser scanning.  Each channel implements the standard OpenSiPM transimpedance amplifier, pole zero cancelation, and low pass filtering to produce a Gaussian single photon response.  

![image](https://github.com/OpenSiPM/sipm-array/assets/16110774/7428e032-695a-4db6-82ce-b01ea915fae4)

# impulse response
![X4-33nh-3 0-30-lpf-470nh-100pf (channel3)](https://github.com/OpenSiPM/sipm-array/assets/16110774/db0ace9f-a296-4e39-b574-1c1a17ab1370)

# power supply
The X4 design uses the standard OpenSiPM power supply and bias generator boards.  Due to the higher current from running 4 SiPMs in parallel, the LT8362 bias generator is recommended for maximum dynamic range, although both designs will work.  Additionally the board can be configured to use two separate power supplies by ommitting resistors and plugging in two supply boards to both sockets.  However, in normal useage this is not required and is probably not useful as the current demand is low enough that a single supply is adquate.

# Non-descanned detection arm
Zemax simulation for non-descanned detection using the 4 channel SiPM board and the prescription for the lens array used can be found [here](https://github.com/OpenSiPM/sipm-array/tree/main/Zemax). 

# publication
A manuscript is forthcoming.  


