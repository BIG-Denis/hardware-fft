# hardware-fft

This repository will contain **parametrized** **pipelined** SystemVerilog implementation for **Fast Fourier Transform** (FFT) based on **radix-2 butterflies** both for **integer and float point** data, **Inverse FFT** (IFFT), SystemVerilog testbenches and Python input sequence generator.  

## Roadmap

Due to project's high complexity progress has been splitted into multiple sequential steps.

1. ⏳ **Vector rotation operator int** - architecture and realisation  
Improving int8 vector rotation operator to work with integers of any width.  
2. 🗓️ **Radix-2 butterfly int** - architecture and realisation  
Improving int8 butterfly to work with integers of any width.  
At this point this would be a MVP.  
3. 🗓️ **Width-parametrized FFT calculation graph** - realisation  
Writing a parametrized size full calculation graph combining all done modules for int FFT.  
4. 🗓️ **Vector rotation operator float point** - architecture and realisation  
Improving vector rotation operator to work with float point data types.  
5. 🗓️ **Radix-2 butterfly float point** - architecture and realisation  
Improving int-only butterfly to work with float point data types.  
6. 🗓️ **DataType-parametrized FFT calculation graph** - realisation  
Parametrizing whole top module to be able to choose data type as module parameter.  
7. 🗓️ **Inverse Fast Fourier transform** - realisation  
Simply rewriting calculation graph to get IFFT algorithm.  

> ✅ - done  
> ⏳ - work in progress  
> 🗓️ - planned  

Documentation is going to be updating as new parts of project will be completed.  
