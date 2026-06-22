# phase-modulation


AIM:
To Simulate the phase modulation (PM) Signal.


EQUIPMENTS REQUIRED

•	Computer with i3 Processor

•	SCI LAB

THEORY:


Phase Modulation (PM) is a type of angle modulation in which the phase of the carrier signal is varied according to the instantaneous amplitude of the modulating signal while keeping the carrier amplitude constant.

In phase modulation, the amount of phase shift introduced in the carrier signal is directly proportional to the amplitude of the message signal. PM is widely used in digital communication systems because of its improved noise immunity and efficient bandwidth utilization.

The message signal is given by:

em = Am cos(2πfmt)

The carrier signal is given by:

ec = Ac cos(2πfct)

The phase modulated signal is given by:

epm = Ac cos(2πfct + β sin(2πfmt))

where,

Am = Amplitude of the message signal
Ac = Amplitude of the carrier signal
fm = Frequency of the message signal
fc = Frequency of the carrier signal
β = Phase modulation index

Thus, in Phase Modulation, the phase of the carrier wave changes in accordance with the message signal while its amplitude remains constant.

Algorithm
1. Start the program.

2. Define the message signal amplitude (Am), message frequency (fm),
   carrier amplitude (Ac), carrier frequency (fc), sampling frequency (fs),
   and phase modulation index (β).

3. Generate the time vector:
      t = 0 : 1/fs : 2/fm

4. Generate the message signal:
      em = Am × cos(2πfmt)

5. Plot the message signal.

6. Generate the carrier signal:
      ec = Ac × cos(2πfct)

7. Plot the carrier signal.

8. Generate the phase modulated signal:
      epm = Ac × cos(2πfct + β sin(2πfmt))

9. Plot the PM signal.

10. Observe the message, carrier, and PM waveforms.

11. Stop the program.

Program
```
Am=12.1;
fm=1632;
Ac=18.15;
fc=16320;
fs=163200;
t=0:1/fs:2/fm;
B=2.7;
em=Am*cos(2*3.14*fm*t);
subplot(4,1,1);
plot(t,em);
ec=Ac*cos(2*3.14*fc*t);
subplot(4,1,2);
plot(t,ec);
efm=Ac*cos((2*3.14*fc*t)+B*sin(2*3.14*fm*t)); 
subplot(4,1,3);
plot(t,efm);
epm=Ac*cos((2*3.14*fc*t)+B*cos(2*3.14*fm*t));
subplot(4,1,4);
plot(t,epm);
```

Output Waveform
<img width="736" height="594" alt="image" src="https://github.com/user-attachments/assets/530ae33f-1f34-4331-85d5-42cd62012e66" />

RESULT:Thus,the simulation for the phase modulation (PM) signal is executed in SCILAB and the output id verified 
