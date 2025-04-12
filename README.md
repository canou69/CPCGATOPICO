# CPC GA TO PICO

Ce projet est en construction et partagé à mon niveau d'avancement sur le projet.  
A ce stade tout est à documenter et succeptible d'évoluer.  
Expérimentation autour des composants 40007 40008 et 40010 de l'Amstrad CPC  

#Création d"un PCB venant se placer entre le support de la puce GA et cette dernière *
-----------------------------------------------------------------------------------------------------------------------------------
Je déconseille vivement de faire une carte à partir des fichiers partagés ici le montage à mis en évidence des problèmes à corriger
-----------------------------------------------------------------------------------------------------------------------------------
Ambitions :  

##Affichage double : 2 modes  
###CPC et Sortie VGA Clone du CPC  
###CPC et Sortie VGA "Menu carte"  
###VGA 5:5:5 (32 niveaux par couleur, 32768 couleurs totales  
##OTG USB, Carte mémoire USB, Clavier..  
##SHELL de monitoring, configuration  
##VERSION CPC (Alimentation CPC, réduction Pcb, orientation sortie etc..)  
  
Divers:  
Remplacement d'un GA (Emulation)  
  
[RP2350B]  
  GPIO0 à GPIO7 ----> D0 à D7 40010  
  GPIO8 ----> CCLK 40010  
  GPIO9 ----> SYNC 40010  
  GPIO10 ----> RESET 40010  
  GPIO11 ----> RAS 40010  
  GPIO12 ----> MWE 40010  
  GPIO13 ----> DISPENS 40010  
  GPIO14 ----> INTERRUPT 40010  
  GPIO15 ----> CASAD 40010  
  GPIO16 ----> HSYNC 40010  
  GPIO17 ----> A14 40010  
  GPIO18 ----> RAMRD 40010  
  GPIO19 ----> VSYNC 40010  
  GPIO20 ----> A15 40010  
  GPIO21 ----> CPU 40010  
  GPIO22 ----> ROMEN 40010  
  GPIO23 ----> CAS 40010  
  GPIO24 ----> MREQ 40010  
  GPIO25 ----> VSYNC VGA D-SUB  
  GPIO26 ----> IORQ 40010  
  GPIO27 ----> 244EN 40010  
  GPIO28 ----> PHY 40010  
  GPIO29 ----> READY 40010  
  GPIO30 ----> M1 40010  
  GPIO31 ----> RD 40010  
  GPIO32 à GPIO36 ----> 5 Bits R-2R couleur bleu B VGA D-SUB  
  GPIO37 à GPIO41 ----> 5 Bits R-2R couleur vert G VGA D-SUB  
  GPIO42 à GPIO46 ----> 5 Bits R-2R couleur Rouge R VGA D-SUB  
  GPIO47 ----> HSYNC VGA D-SUB  
    
  *Note : SYNC était inutile, il aurait été plus judicieux de prendre CK16  
