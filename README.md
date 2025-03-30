# CPCGATOPICO

Ce projet est en construction et partagé à mon niveau d'avancement sur le projet.
A ce stade tout est à documenter et succeptible d'évoluer.
Expérimentation autour des composants 40007 40008 et 40010 de l'Amstrad CP
***************************************************************************************
* Création d"un PCB venant se placer entre le support de la puce GA et cette dernière *
***************************************************************************************
Ambitions :

Affichage double : 2 modes 
  (1.CPC et Sortie VGA Clone du CPC -/- 2.CPC et Sortie VGA "Menu carte")
---------------------------------------------------------------------------------------
Séquence de déblocage ASIC pour envoyer des commandes du CPC au 2350B
---------------------------------------------------------------------------------------
Administration de la carte pilotable depuis le CPC ou via USB vers un PC 
---------------------------------------------------------------------------------------
Affectation des palettes et ajustement des couleurs
---------------------------------------------------------------------------------------
Mode terminal via USB
---------------------------------------------------------------------------------------
Monitoring des pins d'un GA actif
---------------------------------------------------------------------------------------

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


