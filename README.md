# Phase Locked Loop(PLL) IC Design using Sky130 Technology

  ![PLL](https://user-images.githubusercontent.com/88245627/127762911-f0dce654-0948-4562-8e17-5ff6756ee7bc.png)

2-day Online Cloud based Workshop organised by VSD from 31st Aug'21 - 1st Aug'21. The details of the workshop can be found here [here](https://www.vlsisystemdesign.com/pll-design-using-sky130/). Brief documentation is provided below based on the theory and labs performed in these 2 days.

# Table of Contents
  1. [Day1](#Day1) : 
      1. [Introduction to PLL](#Introduction-to-PLL) 
      2. [Introduction to Components of PLL](#Introduction-to-Components-of-PLL)
      3. [Setting Up Lab Environment](#Setting-Up-Lab-Environment)
     
  2. [Day2](#Day2) :
      1. [PLL Component Design and Simulation](#PLL-Component-Design-and-Simulation)
      2. [Combining PLL sub-circuits and full simulation](#Combining-PLL-sub-circuits-and-full-simulation)
      3. [Layout Design](#Layout-Design)
      4. [Tapeout Theory](#Tapeout-Theory)

# Day1 - Introduction to PLL and its components

  ## Introduction to PLL 
  PLL or the Phase Locked Loop checks the ouput phase of a Voltage Controlled Oscillator and compares it with the phase of the input signal. In this workshop, we had to design the   PLL with Google Skywater130nm Technology. The expected output should have good flexibility and should be implementable On-chip.
  
  ## Introduction to Components of PLL 
  The basic components of the PLL are :
  
   1. *Phase Frequency Detector* - It basically compares the input and poutput phases of the signal and give UP and DOWN signals as the output. We can understand the following    
       using the timing diagram shown below.
       
   ![PFD](https://user-images.githubusercontent.com/88245627/127773983-c83f3529-64e8-4e8e-bff7-7b53572b1d35.JPG)
   
   2. *Charge Pump* - It converts the digital measure of phase or frequency difference into an analog control signal to control the oscillator.

   3. *Voltage Controlled Oscillator(VCO) and Frequency Divider* - The Voltage Controlled Oscillator output frequency on the delay and delay depends on the current supplied. The frequency divider circuit comprises of a toggle flip-flop by using D flip-flop and an inverter.

  ## Setting Up Lab Environment -
   In order to set up the tool flow and files for running the lab sessions, the following commands are used. 
      
   ![image](https://user-images.githubusercontent.com/88245627/127774221-16eb44f1-a29c-430b-86ab-75ebeb7a78fc.png)
   
   Cloning this directory, we get all the required Sky130 library files and PDK files to start with out lab.
  
  # Day2 - PLL Lab   
   
   ## PLL Component Design and Simulation
   
   Making a new directory inside the PLL_Work folder named 'work_dir' and keeping the necessary files of sky130 to get the expected results.
  
  ![image](https://user-images.githubusercontent.com/88245627/127774544-0e0b7381-4859-43ea-87f7-3cb3b749a120.png)

  1. *Frequency Division* -
      
      ![image](https://user-images.githubusercontent.com/88245627/127881560-2050d7b1-65a3-4961-8302-3fb76f44fa0d.png)
     *Output* - 
      ![image](https://user-images.githubusercontent.com/88245627/127774673-52487d2f-3ec4-4495-b20f-3e438a57662d.png)
      
   2. *Charge Pump* - 
      
      ![image](https://user-images.githubusercontent.com/88245627/127882766-221587fd-3284-4f1d-ac67-ef214845c8f9.png)
   
      *Output* - 
   
   *Before Adding Pulse* -           
   ![image](https://user-images.githubusercontent.com/88245627/127774776-e6a00743-72f6-42de-bf25-2276189442af.png)
   
   *After Adding Pulse* -      
   ![image](https://user-images.githubusercontent.com/88245627/127774805-9f4a64d6-a48c-437b-a481-a68ad872503e.png)
   
   3. *Voltage Controlled Oscillator* -

      ![image](https://user-images.githubusercontent.com/88245627/127774998-d7b1d119-ffe9-4690-90a9-2fb789559793.png)
      
      *Output* - 
      
      ![image](https://user-images.githubusercontent.com/88245627/127775019-202d34b9-cfa9-4f18-abd8-0b2689eb982b.png)
      
   4. *Phase Detector* - 

      ![image](https://user-images.githubusercontent.com/88245627/127882908-40fc1d4d-7372-423b-86a6-e3c4b1c5f1e0.png)
      
      *Output* - 
      
      ![image](https://user-images.githubusercontent.com/88245627/127775144-6f2da6bb-2901-4d67-9d90-34399e2b2b62.png)
      
   ## Combining PLL sub-circuits and full simulation
  
   *Simulating PLL with all the combined sub-circuits.*
  
   ![image](https://user-images.githubusercontent.com/88245627/127883536-6e505f70-3f51-43b3-bf3b-b5d306327f15.png)
   
   *Ouput* - 
   
   ![image](https://user-images.githubusercontent.com/88245627/127775225-8abcaece-4949-4502-bdc6-560fc270db00.png)
   
   ## Layout
   
   


      
      
      
      
      
      
   ## Acknowledgment
   
   1. Kunal Ghosh
   2. Lakshmi Sathi
   3. VSD-IAT







      
      
      

     

  
  
  


