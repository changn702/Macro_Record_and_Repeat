# Macro_Record_and_Repeat
A Python based program using PyQt to create a GUI which records keystrokes and mouse clicks (at specified areas) to repeat. 

This program (work in progress) was made using Python 3.7.1 with the following libraries: sys, os, pyautogui, json, pandas, time, mouse, and PyQt5. This program was designed for Windows OS.

The program was made originally to automate data entry into a website which does not have a spreadsheet importer to import all results, as well as not having the ability to do multiple entries in one iteration. The program automates this and takes data from a spreadsheet to fulfill all data entry (if a spreadsheet was specified during setup). The automation will repeat until the end of the spreadsheet. 

The program works by allowing you to create your own macro to repeat using the "Input" commands located on the right. The "Action Delay (sec)" in the main window is used to apply a delay after an action (currently allowing anywhere from 0.1 to 19.9 seconds). For example, a delay of 0.1 sec means if you recorded a click, it will then delay 0.1 seconds before the next command and the delay will not change unless the user applies the change. Simply change the delay to desired time (in seconds) and click apply.

"Input Hotkey" allows for recording of keyboard commands such as hotkeys like Ctrl+C (some hotkeys available, will work in progress to create a function for selecting your own hotkeys), keyboard typing, and including excel entries from a specified column in the spreadsheet. By simply clicking on the hotkeys/buttons listed (excluding "entry"), the program will record that key command. Using "Excel Entry" will prompt users to input the column/header name which the program will take the data from. "Typing Entry" will prompt users to input what they would like the program to type at that specified time.

"Input Mouse Controls" only has left click options at the moment (right click to be added in the future) and will allow users to specify the amount of clicks desired at a specific position on the screen. The control works simply by adjusting the number of clicks (if necessary), clicking the record button, then clicking on the position where you would like to record the click (wait a second before moving the mouse from the desired spot). This will record the spot to click on when the program runs.

The current macro in use or in recording will be displayed on the main window under "Current Macro in use". To undo the last recorded entry, you can press the "Undo" button under commands. To save the current macro, click the "Save" button under commands which will save the macro (and the description of the macro in use) into a .JSON file. To restart everything from scratch, press "Reset" under commands.

The program will only do a single iteration if no "Excel Entry" was specified/entered. To prevent accidental repeating, the "Clear At End?" allows a checkbox to make sure to clear the data at the end of the run. 

If loading a presaved Macro and or Excel file, click the "Open" under the respective item in the main menu to load Macro or Excel.

To start macro after loading/creating, simply press "Start Macro" and a 3 second delay will apply before starting the run. 

