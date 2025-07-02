# hardware-fft

This repository will contain **parametrized** **pipelined** SystemVerilog implementation for **Fast Fourier Transform** (FFT) based on **radix-2 butterflies** both for **integer and float point** data, **Inverse FFT** (IFFT), SystemVerilog testbenches and Python input sequence generator.  

## Roadmap

Due to project's high complexity it's progress has been splitted into multiple sequential steps.

1. ⏳ **Vector rotation operator int8** - architercute and realisation  
The main thing in hardware FFT is and vector rotation operator that must be parametrized good enough to comply with giant FFT`s. First step is to make it for ite int8 data type - easiest one.  
2. 🗓️ **Radix-2 butterfly int8** - architercute and realisation  
Next part is a core unit opeation in FFT's - butterfly, which is basically adder, substractor and vector rotation.  
3. 🗓️ **Vector rotation operator int (any width)** - architercute and realisation  
Improving int8 vector rotation operator to work with integers of any width.  
4. 🗓️ **Radix-2 butterfly int (any width)** - architercute and realisation  
Improving int8 butterfly to work with integers of any width.  
At this point this would be a MVP.  
5. 🗓️ **Width-parametrized FFT calculation graph** - realisation  
Writing a parametrized size full calculation graph combining all done modules for int FFT.  
6. 🗓️ **Vector rotation operator float point** - architercute and realisation  
Improving vector rotation operator to work with float point data types.  
7. 🗓️ **Radix-2 butterfly float point** - architercute and realisation  
Improving int-only butterfly to work with float point data types.  
8. 🗓️ **DataType-parametrized FFT calculation graph** - realisation  
Parametrizing whole top module to be able to choose data type as module parameter.  
9. 🗓️ **Inverse Fast Fourier transform** - realisation  
Simply rewriting calculation graph to get IFFT algorithm.  

> ✅ - done  
> ⏳ - work in progress  
> 🗓️ - planned  
