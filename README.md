# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 French
firmware-20231121-011635.bin

# Ender-5 4.2.7 32 bits avec BLTouch Marlin 2.1.2.1 EN 
firmware-20231121-002343.bin

# Ender-5 4.2.732 bits Marlin 2.1.2.1 French
firmware-20231122-003448.bin

# Ender-5 4.2.7 32 bits Marlin 2.1.2.1 EN
firmware-20231120-235233.bin


#define DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 800, 93 }

Mise en place du CRTouch

#define BLTOUCH
________________________________________________

/**
* Enable this option for a probe connected to the Z-MIN pin.
* The probe replaces the Z-MIN endstop and is used for Z homing.
* (Automatically enables USE_PROBE_FOR_Z_HOMING.)
*/
//#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN
// Force the use of the probe for Z-axis homing
#define USE_PROBE_FOR_Z_HOMING
________________________________________________
/**
* Z_MIN_PROBE_PIN
*
* Define this pin if the probe is not connected to Z_MIN_PIN.
* If not defined the default pin for the selected MOTHERBOARD
* will be used. Most of the time the default is what you want.
*
* - The simplest option is to use a free endstop connector.
* - Use 5V for powered (usually inductive) sensors.
*
* - RAMPS 1.3/1.4 boards may use the 5V, GND, and Aux4->D32 pin:
* - For simple switches connect...
* - normally-closed switches to GND and D32.
* - normally-open switches to 5V and D32.
*/
#define Z_MIN_PROBE_PIN PB1 // Pin 32 is the RAMPS default (PB1 is for Z_MIN_PROBE PB1 defined in Marlin>src>PINS>STM32f1>pins_CREALITY_V4.h)

#define Z_CLEARANCE_DEPLOY_PROBE   1 // Z Clearance for Deploy/Stow
