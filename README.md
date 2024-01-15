# Ici les fichiers sont pour une carte mere Creality 32 bits 4.2.7 STM32F103RE.

Vous avez un fichier << Marlin-2.1.2.1.rar >> comprenant la source Marlin retravaillée, avec les dernires modifications:
- multilingue Francais / anglais,
- Silent driver configurés
- BL touch, ou CR Touch ou 3D Touch
- Auto bed leveling avant impression

Avec le également le firmware compilé "pret à flasher" 

# << Ender 5 Marlin firmware cook.docx >>
C'est le fichier pour vous aider à faire votre propre version 
=> Pas à pas pour installer telecherger Marlin 2.1.2.1, les fichiers de configuration propore à votre machine
( suivre le meme pas a pas si vous avez une carte mere 4.2.7, en téléchargeant la version des fichiers Configuration.h et Configuration_adv.h pour votre imprimante)
=> Pas à pas pour personnaliser votre configuration
=> Pas à pas pour compiler votre firmware 

Enjoy 

--


# Le fichier soucrce Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.x French
comming soon

# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.x French
STM32F103RE_creality testé Ok avec CR Touch

firmware-20231221-181654.bin 

# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.x EN 
STM32F103RE_creality testé Ok avec CR Touch

firmware-20231221-184003.bin

# Ender-5 4.2.732 bits Marlin 2.1.x  French
STM32F103RE_creality 
comming soon
# Ender-5 4.2.7 32 bits Marlin 2.1.x EN
STM32F103RE_creality 
comming soon

________________________________________________


# Modifications apportées au code Créality Ender 5: 

#define DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 800, 93 }
________________________________________________

Mise en place du CRTouch

#define BLTOUCH
/#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN

#define USE_PROBE_FOR_Z_HOMING

#define Z_MIN_PROBE_PIN PB1 // Pin 32 is the RAMPS default (PB1 is for Z_MIN_PROBE PB1 defined in Marlin>src>PINS>STM32f1>pins_CREALITY_V4.h)

#define Z_CLEARANCE_DEPLOY_PROBE   1 // Z Clearance for Deploy/Stow
