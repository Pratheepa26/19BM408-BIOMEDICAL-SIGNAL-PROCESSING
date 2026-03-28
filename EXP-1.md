# GENERATION OF STANDARD DISCRETE-TIME SIGNALS
# AIM:
To generate and plot standard discrete-time signals using MATLAB.
# APPARATUS REQUIRED:
•	Computer / Laptop
•	MATLAB software
# THEORY:
Discrete-time signals are signals defined only at integer values of time (n).
These signals are basic building blocks in Digital Signal Processing (DSP) and are used for system analysis, filtering, and signal modeling.
Standard discrete-time signals include:
	Unit Impulse
	Unit Step
	Ramp
	Exponential
	Sinusoidal
	Damped Sinusoidal
In MATLAB, discrete-time signals are represented using vectors and plotted using the stem() command.
 Standard Discrete-Time Signals
 
🔹 1. Unit Impulse Signal
δ(n)={■(1,&n=0@0,&n≠0)┤

🔹 2. Unit Step Signal
u(n)={■(1,&n≥0@0,&n<0)┤

🔹 3. Ramp Signal
r(n)=n⋅u(n)

🔹 4. Exponential Signal
x(n)=a^n

🔹 5. Sinusoidal Signal
x(n)=sin⁡(ωn)

🔹 6. Damped Sinusoidal Signal
x(n)=a^n sin⁡(ωn)

# ALGORITHM:
1.	Start the program
2.	Define the sample index n
3.	Generate each standard discrete-time signal
4.	Plot the signal using stem()
5.	Label the axes and title
6.	Stop the program

# MATLAB CODE:
```
% GENERATION OF STANDARD DISCRETE-TIME SIGNALS

clc;
clear;
close all;

%% Sample index
n = -10:10;

%% 1. Unit Impulse Signal
x1 = (n == 0);
figure;
stem(n, x1, 'filled');
title('Unit Impulse Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 2. Unit Step Signal
x2 = (n >= 0);
figure;
stem(n, x2, 'filled');
title('Unit Step Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 3. Ramp Signal
n1 = 0:10;
x3 = n1;
figure;
stem(n1, x3, 'filled');
title('Ramp Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 4. Exponential Signal
a = 0.8;
x4 = a.^n1;
figure;
stem(n1, x4, 'filled');
title('Exponential Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 5. Sinusoidal Signal
x5 = sin(0.3*pi*n1);
figure;
stem(n1, x5, 'filled');
title('Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 6. Damped Sinusoidal Signal
x6 = (0.9.^n1).*sin(0.4*pi*n1);
figure;
stem(n1, x6, 'filled');
title('Damped Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;
```


# OUTPUT GRAPH:

<img width="719" height="550" alt="Screenshot 2026-03-28 134748" src="https://github.com/user-attachments/assets/4838f487-529e-427a-b37e-ba466f8defe1" />

<img width="705" height="552" alt="Screenshot 2026-03-28 134935" src="https://github.com/user-attachments/assets/a81d4691-e002-4fb2-8ee0-be93433a91ea" />

<img width="713" height="557" alt="Screenshot 2026-03-28 134947" src="https://github.com/user-attachments/assets/febdb5e1-61b2-4b24-947d-53ab080eb17d" />

<img width="704" height="547" alt="Screenshot 2026-03-28 135237" src="https://github.com/user-attachments/assets/b3b05ebf-be6f-4dd3-a2b8-4cea68c77548" />

<img width="714" height="546" alt="Screenshot 2026-03-28 135254" src="https://github.com/user-attachments/assets/3658ee14-23f1-42dc-9d1d-7e4596244131" />

<img width="716" height="538" alt="Screenshot 2026-03-28 135331" src="https://github.com/user-attachments/assets/2fda2aa9-2fef-4401-bc4f-f80bfe541c8f" />







# Result :
Thus, standard discrete-time signals were successfully generated and plotted using MATLAB.



