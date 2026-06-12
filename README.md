# phase-modulation


AIM:
To Simulate the phase modulation (PM) Signal.


EQUIPMENTS REQUIRED

•	Computer with i3 Processor

•	SCI LAB

THEORY:
Phase Modulation (PM) is an angle modulation technique in which the phase of the carrier signal is varied in accordance with the instantaneous amplitude of the modulating signal while the carrier amplitude remains constant.

The phase-modulated signal is given by:

e
PM
	​

=A
c
	​

cos(ω
c
	​

t+βsinω
m
	​

t)

where:

A
c
	​

 = Carrier amplitude
ω
c
	​

 = Carrier angular frequency
ω
m
	​

 = Message angular frequency
β = Phase modulation index

In PM, the phase deviation of the carrier is directly proportional to the amplitude of the message signal.

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

Em=Am*cos(2*3.14*fm*t);
subplot(4,1,1);
plot(t,Em);

Ec=Ac*cos(2*3.14*fc*t);
subplot(4,1,2);
plot(t,Ec);

Efm=Ac*cos((2*3.14*fc*t)+B*sin(2*3.14*fm*t));
subplot(4,1,3);
plot(t,Efm);

Epm=Ac*cos(2*3.14*fc*t-B*cos(2*3.14*fm*t));
subplot(4,1,4);
plot(t,Epm);

```
MODEL GRAPH
 <img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/55326c5b-7dd5-4873-aaf6-d219bb7c4420" />
 TABULATION:
<img width="637" height="332" alt="image" src="https://github.com/user-attachments/assets/7ff79056-9cf7-4ff0-a385-703060457972" />
Calculation
<img width="648" height="362" alt="image" src="https://github.com/user-attachments/assets/07db08ba-635e-410e-914a-efc758fa6b82" />

Output Waveform
<img width="760" height="580" alt="image" src="https://github.com/user-attachments/assets/3efbd926-dbb4-4692-9040-b72d6a7faf32" />

RESULT:
Thus the amplitude modulation and demodulation is experimentally done and the output is verified.
