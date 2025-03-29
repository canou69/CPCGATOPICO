# CPCGATOPICO
Expérimentation autour des composants 40007 40008 et 40010 de l'Amstrad CPC

Etape courante : Attente rèception de la carte

Fait : 
  Proto du PCB
  Commande
RAF :
  Contrôle de base de la carte
  Toute la partie software
  ...

La carte :

Toutes les connections du GA sont interfacées avec les GPIO du Weaxie RP2350B
Sauf : R G B et CK16
dont
15 GPIO sont utilisés pour générer un signal VGA 555 32768 couleurs
2 GPIO pour HSYNC et VSYNC VGA
8 GPIO pour D0-D7
etc

