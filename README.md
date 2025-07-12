# ATmega32-Based-Washing-Machine-Controller
A smart washing machine controller built using ATmega32. Includes multiple washing modes, water level sensors, relays for pump/motor control, a 4x4 keypad, and LCD interface. Simulated in Proteus and implemented in hardware.

# ATmega32 Washing Machine Controller

This project is an embedded systems implementation of an automated washing machine using the ATmega32 microcontroller. It features multiple washing modes, relay-based control for pumps and motor, LCD status display, a 4x4 keypad for input, and water level sensors for safety and automation.

## ⚙️ System Features
- 5 wash modes (Quick, Normal, Heavy, Rinse, Dry)
- 4x4 keypad for user input
- 16x2 LCD for displaying status
- Relays to control inlet/drain pumps and washing motor
- Water level sensors for full/empty tank detection
- Pause/resume functionality using a dedicated key
- Beeper and LEDs for user feedback
- Proteus simulation and real hardware implementation

## 🔌 Hardware Components
- ATmega32 microcontroller
- LCD (16x2, 4-bit mode)
- 4x4 matrix keypad
- 3 relays (motor, inlet, drain)
- 2 digital water sensors (full, empty)
- DC motor / fan
- Buzzer and LEDs

## 🛠️ Tools Used
- C (AVR-GCC)
- Proteus for simulation
- Atmel Studio or any compatible IDE
- External power supply (5V for logic, 12V/220V for motor/pumps)

## ▶️ How It Works
1. LCD displays "WashMachine" and mode menu.
2. User selects mode via keypad.
3. Water fills the drum until the full sensor triggers.
4. Washing cycle runs for a set time based on mode.
5. Drain pump is activated until the tank is empty.
6. Optional spin/dry cycle follows.
7. LEDs indicate each phase; buzzer signals completion.



## 📁 Files
- `main.c`: Embedded code for ATmega32
- `proteus/`: Simulation files
- `schematic.pdf`: Circuit wiring diagram

## 📌 Notes
- LCD connected via PC0–PC5, EN on PD3
- Relays connected to PORTB
- Sensors on PD6 (Full), PD7 (Empty)

## 🧠 Lessons Learned
- Relay and sensor integration
- LCD control in 4-bit mode
- Debounce logic for keypads
- Embedded system design from simulation to hardware

