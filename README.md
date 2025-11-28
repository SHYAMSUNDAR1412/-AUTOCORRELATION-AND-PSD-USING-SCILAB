# AUTOCORRELATION-AND-PSD-USING-SCILAB

# AIM
  TO Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

# APPARATUS REQUIRED
  *Computer with i3 Processor
  
  *SCI LAB

# THEORY

  The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.
  
# Algorithm

1.Load or Define the Signal: Input your time-domain signal.

2.Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.Plot Results: Visualize the autocorrelation function and PSD.

# PROCEDURE
  *Refer Algorithms and write code for the experiment.

  *Open SCILAB in System

  *Type your code in New Editor

  *Save the file

  *Execute the code

  *If any Error, correct it in code and execute again

  *Verify the generated waveform using Tabulation and Model Waveform

  # PROGRAM:
```
t=0:0.01:2*%pi;
x=sin(9*t);
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```
  # OUTPUT:

  <img width="1919" height="1003" alt="Screenshot 2025-11-15 082450" src="https://github.com/user-attachments/assets/8edc30d2-0752-4bd4-b427-3a403a5f3243" />
  
  ![WhatsApp Image 2025-11-28 at 12 15 01_77f9b81c](https://github.com/user-attachments/assets/bdd7b2a5-c472-419c-8c58-744e3aef2313)

  
 # RESULT:
  ![WhatsApp Image 2025-11-28 at 12 15 01_067a5221](https://github.com/user-attachments/assets/2ee237a0-3c61-4e69-a2bf-b1c1fedc0af8)


  

