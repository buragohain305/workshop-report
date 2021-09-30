# workshop-report
# Table of contents
1.	Day1

 a. Introduction
 
 b.  Basic 10-bit DAC design
 
 c. Basic switch design
 
 d. labelling and simulation using eSim
 
2.   Day2

# Day 1

# Introduction

Before going to the designing part of a DAC ckt, we must know the need of an DAC/ADC ckt.

In general every signal around us are in analog form ,but for the signals to be analysed or processed by digital system we need to convert them into digital form. This is where the concept of DAC/ADC comes into picture.

It is more efficient and substantially more accurate to do signal processing in the digital domain (i.e. the language used by computers). Ultimately though, things that interact directly with humans do so in the analog domain (i.e. humans hear sound, not ones and zeros). Therefore, the purpose of a DAC is to take digital domain signal processing results and convert them into a form that is directly or indirectly amenable to humans.

# An n-bit DAC

As the name implies n-bit DAC meaning it can take n-bit digital word as an input and convert them into analog signal in the form of voltage or current.

![image](https://user-images.githubusercontent.com/91653986/135462518-46baeafb-58e3-4605-9fd7-9f7b9a43f6ff.png)


# Potentiometric DAC

Potentiometric DAC is one of the way where we can implement the n-bit DAC.

It uses the cocept of voltage divider.


![image](https://user-images.githubusercontent.com/91653986/135465130-e32c18f7-02b0-4524-88bd-1fcf8762cab3.png)


To understand the working of potentiometric DAC let us consider a 2 bit potentiometric DAC ckt.


![image](https://user-images.githubusercontent.com/91653986/135468697-9c33b6e7-76fd-4cf7-a266-e555ae268663.png)


 so in this 2bit potentiometric ckt let us consider Vref as 4V 
Since R1,R2,R3,R4 are in series so, the voltage Vref will equally distrubuted, i.e V3=3V, V2=2V, V1=1V, V0=0V.
So here the 2 digital inputs are D0 and D1 where D0 is the least significant bit and D1 is the most significant bit.

So let us consider an combination of digital input as  1 0  ,i.e D0=1, D1=0.
So accordingly switch D0 will be closed and D1’ will be closed as a result at output we get 1V

Similarly if we cosider 1 1 , i.e D0=1, D1=1
Switch D0 and D1 both will be closed giving 3v at output.

![image](https://user-images.githubusercontent.com/91653986/135479682-bb1909ca-20cc-4f43-b2b6-6efddae02a38.png)










