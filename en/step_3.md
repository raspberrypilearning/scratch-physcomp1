## Code your circuit

In this step, you will connect your completed circuit to an output pin on the Raspberry Pi and control it using the `Simple Electronics`{:class="block3extensions"} extension.

Our circuit is tested and working, and our LED is on; but we want it to light up when something happens in our Scratch program. 

In order to do that, we need to connect our LED circuit to an output pin on the Pi.

--- task ---
Take the jumper cable off of Pin 1 and attach it to any other numbered Pin. In this example, I’ve used Pin 21 (because it’s easy to get to) but you can use any numbered GP pin on your Raspberry Pi. 


![circuit diagram of a jumper cable with a resistor and LED wired to 3V3 on the Raspberry Pi](images/Pi_21_Complete.png)

If you use a different pin to Pin 21, make sure that you change the number **everywhere** it appears in your code.

--- /task ---

--- task ---

Download and open the premade Scratch project [available here](http://rpf.io/p/en/rpi-scratch-physcomp1-get){:target="_blank"}.

--- /task ---

--- task ---
Make sure you have the **Stage** selected and can see the following scripts:
![Screenshot of scripts. When green flag clicked, ](images/stage_code.png)
--- /task ---
--- task ---
Using the **Simple Electronics** Extension, add the following blocks into the **if** block so that if **distance** is less than 10, the LED comes on - **else** it turns off.
```blocks3
turn LED (21 v) [on v] ::led extension

turn LED (21 v) [off v] ::led extension
```
--- collapse ---
---
title: I need a hint!
---
You want the light to go on if the distance between your sprites gets smaller, and off if it gets larger.

Try:
```blocks3
when green flag clicked
forever
if <[0] < (dist) > then
  turn LED (21 v) [on v] ::led extension
else
  turn LED (21 v) [off v] ::led extension
end
```
--- /collapse ---

--- /task ---

--- task ---
Now click the green flag, and see if you can hunt the hedgehog!
--- /task ---

--- save ---
