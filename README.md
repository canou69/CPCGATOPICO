# CPC GA TO PICO

Ce projet est en construction et partagé à mon niveau d'avancement sur le projet.  
A ce stade tout est à documenter et susceptible d'évoluer.  
Expérimentation autour des composants 40007 40008 et 40010 de l'Amstrad CPC  

## Ambitions (au 27/02/2026)

Sortie VGA :

[ ] Mode 0 Terminal (shell de Monitoring et gestion de la configuration de la carte)

[ ] Mode 1 Clone de la sortie video du CPC
[ ] OTG USB, Carte mémoire USB, Clavier

[X]PCB venant se placer entre le support de la puce GA et cette dernière
Je déconseille vivement de faire une carte à partir des fichiers partagés ici a ce stade du projet

## Le PCB

Le PCB est connecté en "Pigtail" sur le circuit 40010 Gate array du CPC 464

[RP2350B] weact

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

## Liste complète des composants

### BOM principal (LCSC)

| Valeur / Référence | Désignateurs | Boîtier | Quantité | Manufacturer Part | Fournisseur | Référence fournisseur | Prix unitaire | Sous-total |
| --- | --- | --- | ---: | --- | --- | --- | ---: | ---: |
| 100nF | C3, C5, C6, C7 | C0805 | 4 | CT41G-0805-2X1-50V-0.1μF-K(N) | LCSC | C126469 | 0.006 | 0.024 |
| 47Ω | R1, R2 | R0805 | 2 | 0805W8J0470T5E | LCSC | C25315 | 0.002 | 0.004 |
| 8.06kΩ | R3, R12, R17 | R0805 | 3 | 0805W8F8061T5E | LCSC | C19006 | 0.002 | 0.006 |
| 4.02kΩ | R4, R11, R16 | R0805 | 3 | 0805W8F4021T5E | LCSC | C17663 | 0.002 | 0.006 |
| 2kΩ | R5, R10, R15 | R0805 | 3 | 0805W8F2001T5E | LCSC | C17604 | 0.002 | 0.006 |
| 1kΩ | R6, R9, R14 | R0805 | 3 | 0805W8F1001T5E | LCSC | C17513 | 0.002 | 0.006 |
| 499Ω | R7, R8, R13 | R0805 | 3 | 0805W8F4990T5E | LCSC | C17722 | 0.002 | 0.006 |
| SN74CB3T3245PWR | U3, U5, U6, U7 | TSSOP-20 | 4 | SN74CB3T3245PWR | LCSC | C15298 | 1.733 | 6.932 |

### Hors BOM (à acheter séparément)

- Module WeAct RP2350B Core Board (1x)
- Connecteur VGA D-SUB (1x, modèle à confirmer)
- Headers / barrettes de broches 2.54 mm (quantité selon montage)

### Remarques

- Le BOM ci-dessus est extrait du fichier `Hardware/BOM_CPCvgaGA_2025-03-24.csv`.
- Les éléments non assemblés (headers, D-SUB, etc.) ne sont pas inclus dans le BOM principal.
