# DigitalClock
**Live_Digital_clock_using_javascript:** <br>
Clocks are useful elements for any UI if used in a proper way. Clocks can be used on sites where time is the main concern like some booking sites or some app showing arriving times of trains, buses, flights, etc. The clock is basically of two types, Analog and Digital. We will be looking at making a digital one. 

  **Approach:** The approach is to use the date object to get time on every second and then re-rendering time on the browser using the new time that we got by calling the same function each second. 

**HTML:** In this section, we have a dummy time in the format of “HH:MM:SS” wrapped inside a “div” tag. 

**CSS:** For CSS, we have just aligned our clock to the center of the page. Other than that, it is just some font-size and width which you can adjust according to your need.

**Note:** You can use digital fonts available online to make the clock look more beautiful. For that, you have to download their file into your project and then use the “font-face” property to use that custom font.

**JavaScript:** For JavaScript, follow the below-given steps.

- Step 1: Create a function “showTime”. <br>
- Step 2: Create an instance of the Date object. <br>
- Step 3: Using the methods of the Date object get “hours”, “minute” and “seconds”. <br>
- Step 4: Set AM/PM depending on the hour value. The Date object works on the 24-hour format so we change the hour back to 1 when it gets larger than 12. The AM/PM also changes according to that.<br>
- Step 5: Now make a string using the same HH:MM:SS format changing the hour, minute, and a second value with the values, we get from Date object methods.<br>
- Step 6: Now replace the string variable in the “div” using the innerHTML property.<br>
- Step 7: To call the function every second use setInterval() method and set the time-interval as 1000ms which is equal to 1s.<br>
- Step 8: Now call the function at the end to start the function at the exact reloading/rendering time as setInterval() will call first after 1s of rendering.
