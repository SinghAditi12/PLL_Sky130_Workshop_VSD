# Phase Locked Loop(PLL) IC Design using Sky130 Technology

  ![PLL](https://user-images.githubusercontent.com/88245627/127762911-f0dce654-0948-4562-8e17-5ff6756ee7bc.png)

2-day Online Cloud based Workshop organised by VSD from 31st Aug'21 - 1st Aug'21. The details of the workshop can be found here -> https://www.vlsisystemdesign.com/pll-design-using-sky130/?awt_a=5L_6&awt_l=9Us3R&awt_m=3jzon6f2f87yw_6. Brief documentation is provided below based on the theory and labs performed in these 2 days.

# Table of Contents
  1. [Day1](#Day1) : 
      1. [Introduction to PLL](#Introduction-to-PLL) 
      2. [Introduction to Components of PLL](#Introduction-to-Components-of-PLL)
      3. [Setting Up Lab Environment](#Setting-Up-Lab-Environment)
     
  2. [Day2](#Day2) :
      1. [PLL Component Design and Simulation](#PLL-Component-Design-and-Simulation)
      2. Combining PLL sub-circuits and full simulation
      3. Layout Design

# Day1 - Introduction to PLL and its components

  ## Introduction to PLL 
  PLL or the Phase Locked Loop checks the ouput phase of a Voltage Controlled Oscillator and compares it with the phase of the input signal. In this workshop, we had to design the   PLL with Google Skywater130nm Technology. The expected output should have good flexibility and should be implementable On-chip.
  
  ## Introduction to Components of PLL 
  The basic components of the PLL are :
  
   1. Phase Frequency Detector - It basically compares the input and poutput phases of the signal and give UP and DOWN signals as the output. We can understand the following    
       using the timing diagram shown below.
       
   ![PFD](https://user-images.githubusercontent.com/88245627/127773983-c83f3529-64e8-4e8e-bff7-7b53572b1d35.JPG)
   
   2. Charge Pump - 
   3. Voltage Controlled Oscillator(VCO) and Frequency Divider-

  ## Setting Up Lab Environment -
   In order to set up the tool flow and files for running the lab sessions, the following commands are used. 
      
   ![image](https://user-images.githubusercontent.com/88245627/127774221-16eb44f1-a29c-430b-86ab-75ebeb7a78fc.png)
   
   Cloning this directory, we get all the required Sky130 library files and PDK files to start with out lab.
  
  # Day2 - PLL Lab   
   
   ## PLL Component Design and Simulation
   
   Making a new directory inside the PLL_Work folder named 'work_dir' and keeping the necessary files of sky130 to get the expected results.
  
  ![image](https://user-images.githubusercontent.com/88245627/127774544-0e0b7381-4859-43ea-87f7-3cb3b749a120.png)

  1. Frequency Division - 
      
      ![image](https://user-images.githubusercontent.com/88245627/127774365-b963facc-b693-4a8a-a3c9-dc7a7757cade.png)
      ![image](https://user-images.githubusercontent.com/88245627/127774644-a2a104ad-d375-4897-b358-cac47b75f51e.png)
  Output - 
      ![image](https://user-images.githubusercontent.com/88245627/127774673-52487d2f-3ec4-4495-b20f-3e438a57662d.png)
      
   2. Charge Pump - 
      
      ![image](https://user-images.githubusercontent.com/88245627/127774730-de25cb3c-4832-48c4-991f-b377cf6eb6f7.png
      ![image](https://user-images.githubusercontent.com/88245627/127774749-f9a44e0d-b463-4595-bf7b-dcd933ce5c6d.png)
   Output - 
      Before Adding Pulse - ![image](https://user-images.githubusercontent.com/88245627/127774776-e6a00743-72f6-42de-bf25-2276189442af.png)
      After Adding Pulse - ![image](https://user-images.githubusercontent.com/88245627/127774805-9f4a64d6-a48c-437b-a481-a68ad872503e.png)





      
      
      

     

  
  
  


