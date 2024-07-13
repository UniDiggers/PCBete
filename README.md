# PCBete

Création d'un PCB pour la robotique.

## Objectif :

Carte électronique ESP32-S3-WROOM-U1 permettant de controller 
- Jusqu'à 3 NEMA 17 
- 3 Capteurs TOF VL53L0X (i2c)
- 1 écran OLED 0.96 128*64 (i2c) 
- Buzzer
- LiDAR*

Alimentation via PowerBank 5Ah avec 5V/3A vers la carte en Type-C vers Type-C .

## Consommation théorique 

**3000mA** sont disponibles :

1x ESP32 environ **150mA**
3x NEMA 17 environ **2400mA**
3x TOF VL53L0X environ **60mA**
1x Ecran OLED environ **15mA**
1x Buzzer environ **10mA**

**TOTAL THEORIQUE : 2635mA / 87%**
*Ce calcul ne prend pas en compte la consommation théorique des composants soudés à la carte.

*le LiDAR est un accessoire optionnel qui peut être ajouté si la consommation instantanée le permet.
1x LiDAR environ **150mA**

TOTAL THEORIQUE avec LiDAR : **2785mA / 92%**

## Temps d'utilisation théorique

Energie Batterie = Capacité (Ah) x Tension sortie ( Volt)
Energie Batterie = 5Ah x 5 = **25Wh**

Temps d'utilisation (heure) = Energie Batterie (watt-heures) / Courant de décharge constant (Ampère)
Temps d'utilisation (heure) = 25Wh / 3A = **8.33 heures**
