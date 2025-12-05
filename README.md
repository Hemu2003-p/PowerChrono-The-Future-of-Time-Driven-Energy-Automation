# PowerChrono-The-Future-of-Time-Driven-Energy-Automation
PowerChrono – Time-Driven Energy Automation System Developed an embedded system using LPC2148 to automate electrical loads based on RTC schedules. Implemented a menu-driven LCD–keypad interface to edit real-time values and configure device ON/OFF timings with full input validation and interrupt-based control.
PowerChrono — Time-Driven Energy Automation System

PowerChrono is an embedded system project designed to automate electrical devices based on Real-Time Clock (RTC) schedules. It allows users to view and modify time, set ON/OFF schedules, and control loads intelligently, helping industries reduce energy wastage and automate repetitive operations.

Features:
Displays real-time date & time using RTC on a 16x2 LCD
Allows RTC editing using a 4×4 matrix keypad
Supports setting device ON/OFF times
Automatically controls loads (LED/device) based on programmed schedule
External switch interrupt for entering EDIT mode
Input validation (hours/min/sec/day/date/month/year ranges)
Multiple editable menus with scrolling navigation (optional advanced modes)

Hardware Requirements:
LPC2148 Microcontroller
16×2 LCD Display
4×4 Matrix Keypad
RTC Module
LED / Device Load
Switch (for interrupt)
USB-UART Converter / DB9 Cable

Software Requirements:
Embedded C
Keil / Any ARM IDE
Flash Magic (for flashing LPC2148)

Project Workflow:
Initialize RTC, LCD, keypad, interrupt, and peripherals
Continuously read RTC and display on LCD
Compare current time with ON/OFF time
Control device state automatically
On switch interrupt → open EDIT MENU

User can:
Edit RTC info
Edit Device ON/OFF Time
Exit to main loop

All inputs validated before updating RTC or control variables
Menu System

Main Edit Menu
1. EDIT RTC INFO
2. EDIT ON/OFF TIME
3. EXIT

RTC Edit Options
Hour
Minute
Second
Day
Date
Month
Year
Exit

ON/OFF Time Edit Options
Device ON Time
Device OFF Time
Exit

CONNECTIONS:
To execute this we want to connect the following as per code written
1.connect port 0,pin number 1 to 0.1 pin to switch to act as interupt.
2.connect lcd data pins from p0.8-p0.16.
3.connect 4X4 matrix pins from p1.16-p1.23.
4.connect pin number p0.5 to led.
5.connect lcd rs and lcd rw to p0.17,p0.18.
6.connect pin number p0.6 to switch to know about the on time and off time.

