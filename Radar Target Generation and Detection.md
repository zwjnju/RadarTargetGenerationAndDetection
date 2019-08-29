# Radar Target Generation and Detection

标签（空格分隔）： 未分类

---

#This project has been divided into several parts:
1. Parameters setting
2. FMCW signal genaration
3. Echo generation
4. Range measurements
5. Range doppler measurements
6. CFAR
## Parameters setting
    In this part, all parameters are setted in the code, including the initial position and velocity of target.
##FMCW signal generation
    In this part, the operating frequency is 77e9 and the cells of range is 1024 and the cells of doppler is 128
##Echo generation
    In this part, I am confused that how to generate the Tx and Rx. Tx is the repetition of every time duration Tchirp, so I use the 'mod' function to preprocess t(i). For Rx, I also consider the arrival time of every t(i). However, the result is not the same as the directly calculate Tx and Rx without preprocessing of t(i). I want to know the reason.
##Range measurements
    I wonder why this part is taken? The range doppler responds have calculated the range measurements
##Range doppler measurements
    This part has been already pre-completed.
##CFAR
    In this part, I set the trainning cells along x and y as Td and Tr, guarde cells as Gd and Gr. The noise_level is calculated by the condision'if(p<Tr-Gr-1 || q<Td-Gd-1)', and the offset is set to 20. I have create a matrix named 'cfar' the same size of RDM, so there is no need to modify RDM.

##It seems my result is not the same as the output in the classroom, where should I improve?




