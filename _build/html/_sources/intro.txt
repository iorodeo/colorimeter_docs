Introduction
==================
Colorimeters are analytical devices commonly used in science labs to measure the concentration of a solution from its light absorbing properties. Colorimeters are extremely useful and flexible lab instruments for a wide range of science education labs.  Some examples of how they are used include:

* Color and absorbance  - Investigate the relationship between the color of a substance and absorption of light at different wavelengths. See :ref:`lab1_label`
* Beer’s Law - Investigate the relationship between concentration and absorbance using colored solutions (eg. food dye, copper sulfate). Calculate molar extinction coefficient. See :ref:`lab2_label`
* Nitrogen cycle - Quantify the breakdown (oxidation) of ammonia into nitrite and nitrate by nitrification bacteria. See :ref:`lab3_label`
* Water quality - Measure several water parameters such as turbidity, chlorine content, pH, water hardness, phosphate content and more;
* Population growth - Measure the turbidity of a microbial culture over time, which serves as an indicator of population growth;
* Enzyme kinetics - Measure the activity of an enzyme over time, even under different environmental conditions (temperature, pH, inhibitors, substrate);



The Educational Colorimeter essentially consists of an RGB LED and a color sensor in a light-tight enclosure which is connected to an Arduino via a colorimeter shield.


.. figure:: image_02.png
   :align:  center



A cuvette holder in the center of the light-tight enclosure properly positions the sample between the LED and the light sensor. When the Educational Colorimeter is operating, the RGB LED illuminates one side of the sample in the cuvette using one of three different wavelengths of light: 625 nm (red), 528 nm (true green) and 470 nm (blue). Light transmitted through the sample passes through a slit on the inner wall of the enclosure to the light sensor. Absorbance of the sample in the cuvette is determined by comparing the intensity of incident light to the intensity of transmitted light as follows:  

.. math::  

   \mathrm{Incident \hspace*{3px} light} = I; \hspace*{10px} \mathrm{Transmitted \hspace*{3px} light} = I_0

.. math::  

   \mathrm{Absorbance} = log_{10} (I/I_0)

.. figure:: image_03.png
   :align:  center



The Educational Colorimeter uses eight (8) digital signals for normal operation. The provided Arduino shield connects 8 digital input-output (DIO) pins of the Arduino microcontroller board with the light sensor and RGB LED.


.. figure:: image_04.png
   :align:  center







