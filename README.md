# DebounceForStopButtonOnSonyRemote

A humble software developers attempt to write the perfect button.

I learned some about circuit analysis this year, so this circuit with a button in it uses the hardware tricks to make a button stay at it's ground reference until it is pressed and then go high consistantly for about .09 seconds. That's the hardware goodness.

I applied ISRs to the button triggered with change (High to Low, or Low to High) and then adjust states accordingly. There are 4 states: READY (and waiting), PRESSING (the button is currently being pressed, but has not been released), PRESSED (the button was pressed and released withing .4 seconds, and HELD (the button was pressed and held down for more than .4 seconds). That's the software goodness.

No it's not amazing, but it is small and perfect and you are welcome to use it for your own applications. I'm putting it up here on the GitsHubs so that I don't ever have to figure it out again.
