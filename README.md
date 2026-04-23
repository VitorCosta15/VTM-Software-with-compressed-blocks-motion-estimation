#VTM-Software-with-compressed-blocks-motion-estimation

#Author: Vítor Silva da Costa
#Federal University of Pelotas

This custom version of the VTM software was modified to apply the proposed Block Compression Algorithm to both the Search Area and the Coding Block during VVC motion estimation, which represents a fundamental stage of my undergraduate thesis.

The modifications were implemented in the file Lib/EncoderLib/InterSearch.cpp, where each 4×4 Coding Block and 4×4 Candidate Block is compressed from 128 bits into 32-bit vectors.

This approach was developed to reduce the memory usage and processing costs of dedicated hardware architectures for VVC motion estimation.

This software simulation enables the evaluation of coding-efficiency losses and memory-access reductions resulting from the proposed approach compared to the baseline implementation of the VTM software.

The full results of this research can be found in the following papers:

https://doi.org/10.29292/jics.v20i1.964
https://doi.org/10.1109/SBCCI66862.2025.11218658
https://github.com/VitorCosta15/SAD-operating-unit-for-VVC-Motion-Estimation (the full undergraduate thesis is available here)

The VHDL implementation of the proposed architecture can be found here:

https://github.com/VitorCosta15/SAD-operating-unit-for-VVC-Motion-Estimation
