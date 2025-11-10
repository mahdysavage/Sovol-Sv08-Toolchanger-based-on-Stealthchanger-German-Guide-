# -Sv08-Toolchanger-basierend-auf-Stealthchanger-Anleitung-

Hier findest du einen StepfürStep-Anleitung/Readme für den Umbau eines Toolchanhger des Sovol Sv08. 

***Bitte beachten***
***Es handelt sich hier um eine Kurzanleitung, es werden zu manchen Themen wie z.B. Mainline Klipper lediglich Hilfefstellungen gegeben***



Step 1: Sv08 auf Toolchanger vorbereiten

      1.1 Mainline Klipper installieren und den eMMc auf 32 GB erweitern
      
      ***Wichtig*** 
      Wenn man vor hat den Toolhead komplett zu verändern bzw. den orginalen nicht nutzen möchten dann kann man das programmieren des Toolboard auslassen.
      Ich habe für meine zukünfitgen Druckköpfe den Bigtreetech ebb36 genommen, wo wir später Katapult bzw. Klipper sowieso installieren. Wenn man aber möchte dass der Drucker nach Mainline-Klipper erst einmal weiter druckt, dann bitte den Video-Guide komplet                  durchfführen. 

      Video-Anleitung:
      https://www.youtube.com/watch?v=1GHY9XKG7DQ
      
      Materialien:
      https://tinyurl.com/MKS-EMMC-32GB-Adapter
      https://tinyurl.com/St-Link-v-2

      


Step 2: Jetzt kommen wir zum Toolchanger, diese Section wird unterteilt in Hardware und Software

-------------------------------
      Hardware zu erst
-------------------------------
      2.1 Netzteil auf min.350watt erweitern

      Video-Anleitung:
      https://tinyurl.com/Netzteil-Verkabelung

      Druck-Teile:
      https://tinyurl.com/Netzteil-Befestigung
      
      Materialien:
      https://tinyurl.com/Meanwell-350watt-Netzteil

      Bild-Verkabelung:
      https://ibb.co/Y73YVfmb

      Tipps von mir: 
      ;achtet auf die Kabeldicke ich empfehle 12AWG also ein Kabelquerschnitt von min. 2.00mm2 
      
      

      2.2 Rahmen für die Toolhead Docks anfertigen

      Materialien/Guide findet ihr in den nachfolgenden link, dort wird alles ausführlich erklärt.

      Komplette Anleitung für den Rahmen:
      https://tinyurl.com/Toolhead-Frame-Bar

      Wenn man ein Voron-Bed einbauen möchte, empfiehlt sich den Nozzlebrush in der Mitte zusetzen!
      Druckteile  in der Mitte Voron Bed:
      https://tinyurl.com/Toolhead-Frame-Bar-Voron

      Tipps von mir: 
      ;Auf die Einkerbung der 2020 Rahmen achten, es müssen keine Misumi sein. Ich empfehle den Schnitt mit einer Kapp-und Gehrungssäge
      ;Richthöhe des horizontalen Profil ca 10cm vom Top des Gehäuse
      ;Druckteile sollte mindestens mit PETG gedruckt werden besser ABS/ASA


      
      2.3 Toolhead aussuchen und Docks einbauen
      Wenn man sich entschieden hat welchen Toolhead man nutzen möchte, kann man die dazu gehörigen Docks wählen. Das ist ganz individuell!! Da der Rahmen eine einzigartige Lösung ist, sollte man ein passgenaues Dock suchen.

      Ich nutze den Anthead Toolhead und dafür den passenden Dock! Ich bin sehr begeistert und kann es jedem empfehlen. Super einfache Montage, gute Dokumentatiion und eine riesen vielfalt an Extruder bzw Hotend Möglichkeiten.
      In meinem fall nutze ich den 5x LGX Lite Extruder mit den 5x Bambulab X1C Hotend. Ich fand die Simbiose aus komplett Alu Extruder mit Bambu Druckqualitöt cool, aber ihr könnt jedes Toolhead anders wählen. Heute würde ich warscheinlich einen LDO Orbiter mit einem         e3d revo oder einen rapido uhf verbauen.

      Anthead / Dock genaueres findet ihr in der Anthead section im main header
      https://github.com/PrintersForAnts/AntHead
      https://tinyurl.com/Anthead-Dock

      Weitere Toolhead Varianten die für mich in Frage gekommen wären, bei denen aber kein passendes Dock dabei war. 
      ***Mit CAD könnte die orginal File einfach auf den Rahmen umgeändert werden***

      https://tinyurl.com/Dragon-Burner
      https://tinyurl.com/Voron-Stealtburner
      https://github.com/Armchair-Heavy-Industries/A4T
      
      Dock Varianten:
      https://github.com/DraftShift/ModularDock


      Tipp von mir:
      ;Achtet auf die kürzere Version der Docks (man spart wichtigen Druckraum :D)
      ;docks und toolhead sollten schon in ABS/ASA gedruckt werden; Druckeinstellung 3 Wände, 20% Infill und Füllmuster Infillart Gyroid
      ;der Dock nutzt ein nozzle blocker der später beim drucken sehr wichtig ist, achte auf sehr hitze beständiges Silikon.
      ;ich kann das Piano Draht nicht empfehlen nehmt hier immer die Sprungstahl Variante da es das Kabel besser Stramm hällt.
      


***Wichtig*** 
***Wir wollen erst einmal einen Toolhead zum laufen bekommen, die Weiteren dann Step by Step. Man kann, wenn man möchte die Hardware bereits auf die gewünschte Anzahl vorbereiten***

