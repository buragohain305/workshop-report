# workshop-report on short time training program on VLSI
# Table of contents
1.	Day1

     a. Introduction
 
     b.  Basic 10-bit DAC design
   
     c. Basic switch design
   
     d. labelling and simulation using eSim
 
2.   Day2

     a. Basic 2-bit DAC implementation using esim and sky130 PDKS

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

# Designing of basic switch using eSim and simulation

![image](https://user-images.githubusercontent.com/91653986/135657329-ab4c5be2-16e8-40be-a701-7831af662ce6.png)



![Screenshot (176)](https://user-images.githubusercontent.com/91653986/135659253-153982df-f912-40a3-9274-2094418891b4.png)




# Working of basic switch
From above simulation and schematic we can observe that when the digital input is high then output of 1st inverter ckt  will be 0 and accordingly the output of 2nd  inverter ckt will be 1



![image](https://user-images.githubusercontent.com/91653986/135658203-89471ddb-e930-40c1-8dd6-9d61db53b5ce.png)


So in below section of the ckt input for  1st inverter ckt  is 0 so o/p will be vin_1 
And input for 2nd inverter ckt is 1 hence nmos will be on as a result giving o/p as vin_1

So when digital input is high we get an high reference voltage(vin_1) and vice versa.  

# Basic 2-bit DAC implementation using esim and sky130 PDKS




![image](https://user-images.githubusercontent.com/91653986/135658931-6a22c266-cbe7-4e3c-9482-8ece2e458e00.png)

schematic of 2-bit DAC



![Screenshot (177)](https://user-images.githubusercontent.com/91653986/135659634-580ca5ac-440f-475a-bfeb-0416c1e85846.png)

simulation of 2-bit DAC


# conclusiom
During this sttp on VLSI I got the opputinity to learn the way to desing or simulate a ckt using eSim and Sky130 PDKS which i think would definitely going to be an important skill for my coming my future or career , so in this report i have mentioned about the designing and simulation of basic switch and 2bit DAC. similarly i would definitely going to implement this knowledge and skills in designing more such ckts like higher order DACs.  


