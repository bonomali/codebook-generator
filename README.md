# IEEE 802.11ad Codebook Generator Application
This repository contains a MATLAB application for generating codebook samples for ns-3 IEEE 802.11ad model. These codebook samples are imported into ns-3 using the Parametric Codebook class.

## Features:
1. With this application, the user can choose either among a set of MATLAB phased antenna array models such as ULA, UCA, and URA or upload a custom steering vector obtained from antenna measurements. 
1. The user can visualize the 2D/3D directivity of the antenna array and define the parameters of each sector and custom AWVs independently. 
1. When using MATLAB phased antenna array models, the user can select between different set of antenna elements such as omni-element, micro-strip, etc. Whereas in the case of custom phased antenna arrays, the steering vector already compromises the effect of antenna element pattern. 
1. The ns-3 Parametric Codebook class parses the file generated by the application and automatically calculates and stores the directivity of each sector and AWV according. 
1. The decoupling of the antenna response and the weights of the antenna elements allows the user to adapt the beam pattern within the course of the simulation based on the the state of the wireless channel. For example, the user can suppress interference and have a null in the direction of a certain station while increasing the power towards the intended receiver. Simulations utilizing the Parametric Codebook involves high computations due to the matrix operations which in turn increases the run-time compared to the other two codebooks. 


Here is a sample snapshot for our Codebook Generator Application:

![Snapshot for our Codebook Generator App](CodebookSnapshot.png)

# Download Information:
We plan to release the App to the public around June 2019.

# Author Information:
The IEEE 802.11ad Codebook Generator Application is developed and maintained by [Hany Assasa](http://people.networks.imdea.org/~hany_assasa/). For more information about my research work, please check my personal website.
