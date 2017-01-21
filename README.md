# pitemp
pitemp - A script that displays the current temperature of a Raspberry Pi system from the onboard SoC.
---

Pitemp is a simple BASH shell script that allows easy access to the current temperature of the SoC (CPU) in a Raspberry Pi computer.  It was written with the following concepts in mind:

* Make it easy to read the current temperature.
* Sane default behavior: Output a single temperature value in Celcius, with a "°C" suffix, then exit.
* Allow the user to customize the command's output and behavior as follows...
  * Output degrees in Fahrenheit instead of Celcius.
  * Set the temperature output to numeric-only (no degrees, "F" or "C" suffixes displayed).
  * Add a timestamp prefix in either UTC or local time for logging purposes.
  * Run the command indefinitely in a delay loop to allow for monitoring of system temperature over time.
  * When running in a loop, allow control of how often the temperature is checked and displayed.

## Installation Instructions:

1. Clone this project, or save the contents of the `pitemp` file to your local Raspberry Pi.
2. Copy the `pitemp` file into a location on your Pi's PATH. (I suggest `sudo cp pitemp /usr/local/sbin`).
3. Change the `pitemp` file's mode to allow for execution of it as a command: `chmod +X pitemp`.
4. Change directory back into your home folder: `cd ~`
5. Test `pitemp` by asking it for the temperature: `pitemp [ENTER]`
6. Finally, obtain usage information by typing `pitemp --help`
