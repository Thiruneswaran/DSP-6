# DSP-LAB-6

#FREQUENCY ANALYSIS OF DFT

PROGRAM:

 clc; 
clear  all; 
x=input ('Enter the sequence :');  
n=length (x); 
y=fft(x,n);  
di sp('output  sequence is:');  
disp(y); 
m=abs(y); 
disp('magnitude function is:');  
disp(m); 
p=angle(y); 
disp('phase  function  is:’); 
disp(p); 
subplot(1,3,1);  
t1=0 : n-1; 
stem(t1,x);  
xlabel('n-->'); 
ylabel('amplitude -->');  
title('input sequence'); 
subplot(1,3,2); 
t2=0 : n-1; 
stem (t2,m);  
xlabel('n-->'); 
ylabel('amplitude -->'); 
title('magnitude plot');  
subplot(1,3,3); 
t3=0 : n-1; 
stem(t3,p);  
xlabel('n-->'); 
ylabel('phase -->');  
title('phase  plot');
# DSP-6
