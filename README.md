
DATE : 21ST May , 2015 , 9:00 PM 	

#MAJOR OS 
#V1.0 (NO WORDS ABOUT FUTURE UPDATES AT THIS MOMENT)
	
--------SOLELY DEVELOPED BY AMIT SINGH RAWAT(amitsrawat28@gmail.com)
	


#TO DO 

**ADD SHUTDOWN COMMAND[MANDATORY]				------->	DONE !

**ADD OPEN SAVED FILE[MANDATORY]				------->	DONE !

**UPDATE DIRECTORY COMMAND [MANDATORY]		-------> 	DONE !

**ADD DELETE COMMAND [OPTIONAL]					------->	AFTER EXAM and BEFORE SUBMISSION OF THE PROJECT	(Exam is on 27th and then 29th May , BACKLOGS;)
**ADD COPY COMMAND [OPTIONAL]					  ------->	AFTER EXAM and BEFORE SUBMISSION OF THE PROJECT (----same as above-----)

**EDIT COMMAND TO CREATE TEXT FILE AND SAVE			-------> 	DONE !

**OPEN COMMAND TO OPEN AND PRINT SAVEDTEXT FILE 		------->	DONE !

**HELP COMMAND							------->	DONE !

**VERSION AND AUTHOR COMMAND					------->	DONE !


#STABLE FEATURE	

*HELP

*DIR

*CLEAR

*EDIT---->TEXT EDITOR---> SAVES FILE ON DISK---> UPDATE DISK MAP---> FEED FILE INFO IN DIRECTORY TABLE

*VERSION

*AUTHOR

*OPEN

*SHUTDOWN

	
#BUGS


** While PUSHing within a shell function and not POPing within that function made CS:IP to point to the start of the shell(i.e later PUSHed items were being considered as IP) ------ NOW FIXED  :)  :D

** Call implicitly push the Current IP to stack and retrieve it with pop.
(With this bug , I came to know about how a CS:IP changes and why we can't manipulate it directly)

** NOT DOCUMENTED YET (Can be considered as a bug nowadays and also WHEN PROGRAMMING IN ASSEMBLY), I will be documenting in near future.


	#DISK STRUCTURE

 BOOTLOADER 	----  SECTOR 1	
 DISK MAP	----  SECTOR 2	
 DIRECTORY	----  SECTOR 3
 KERNEL		----  SECTOR 4
 SHELL    	----  SECTOR 5   to  SECTOR 16
 USER FILES	----  SECTOR 17  to  *MAX SECTOR(512)
      	     	                    
*MAX SECTOR ----- DEPENDS ON THE DISK YOU WRITE THIS OS CODE

				#SIZE--------------
  

			BOOTLOADER  	= 	512 BYTES
   
			DISK MAP    	= 	512 BYTES
   
			DIRECTORY   	= 	512 BYTES
   
			KERNEL	   	= 	512 BYTES
   
			SHELL	   	= 	6KB (12 SECTORS)
   
			USER FILES  	= 	MAX 1KB

# I know, my code is redundant by not using any 16-bit linker , and I guess NASM doesn't produce 16-bit object code 
 
