# AM-USING-PYTHON

## Aim


To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. 

## Apparatus Required

1.	Software: Python with NumPy and Matplotlib libraries
2.	Hardware: Personal Computer
  
## Theory

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. The general form of an FM signal is:

## Algorithm


1.	Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and frequency deviation.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
5.	Generate AM Signal: Apply the AM modulation formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

## Program
```
import numpy as np
import matplotlib.pyplot as plt
Am = 7
fm = 447
Ac = 14
fc = 4470
fs = 44700
t = np.arange(0,2/fm,1/fs)
m=Am*np.cos(2*np.pi*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)
c=Ac*np.cos(2*np.pi*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)
s=(Ac+Am)*np.cos(2*np.pi*fc*t)
plt.subplot(3,1,3)
plt.plot(t,s)

```

## Output Waveform

<img width="687" height="517" alt="image" src="https://github.com/user-attachments/assets/73e2f550-5bdc-499d-a7f3-c9cbe9fcdada" />





## Tabular Column

![WhatsApp Image 2025-11-29 at 06 47 05_070e18e2](https://github.com/user-attachments/assets/03e03210-5777-4672-b35e-3bcc81d03cee)


## Result

The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. The modulated signal will show amplitude variations corresponding to the amplitude of the message signal.

