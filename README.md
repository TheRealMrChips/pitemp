# pitemp
pitemp - A script that displays the current temperature of a Raspberry Pi system from the onboard SoC.
---

Pitemp is a simple BASH shell script that allows easy access the current temperature of the SoC (CPU) in a Raspberry Pi computer.  It was written with the following concepts in mind:

* Make it easy to read the current temperature.
* Allow the user to customize the command's output and behavior as follows...
  * Output degrees in Fahrenheit instead of Celcius.
  * Set the temperature output to numeric-only (no degrees, "F" or "C" suffixes displayed).
  * Add a timestamp prefix in either UTC or local time for logging purposes.
  * Run the command indefinitely in a delay loop to allow for monitoring of system temperature over time.
  * When running in a loop, allow control of how often the temperature is checked and displayed.
* Sane default behavior: Output a single temperature value in Celcius, with a "°C" suffix, then exit.
