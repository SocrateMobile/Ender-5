Ici les fichiers sont pour une carte mere 32 bits STM32F103RE.
Pour la STM32F103RE_creality, il faudra le compiler, ou me le demander 


# Le fichier soucrce Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 French
MarlinCRT OK.zip

# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 French
STM32F103RE_creality testé Ok avec CR Touch
firmware-20231125-152215.bin

# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 EN 
STM32F103RE_creality testé Ok avec CR Touch
firmware-20231125-153959.bin

# Ender-5 4.2.732 bits Marlin 2.1.2.1 French
STM32F103RE_creality firmware-20231122-003448.bin

# Ender-5 4.2.7 32 bits Marlin 2.1.2.1 EN
STM32F103RE_creality firmware-20231120-235233.bin


________________________________________________

#  Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 French
STM32F103RC_creality firmware-20231205-014339.bin


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
