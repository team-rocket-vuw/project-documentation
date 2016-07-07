# Style guide for embedded code

Due to the open source nature of this project, and the fact that initial sketches are based off Arduino code structure, code will be written to conform with the Arduino styleguide.

The style guide loosely followed can be found [here](https://www.arduino.cc/en/Reference/StyleGuide). This styleguide will be applied to the __main sketch__ per launch.

To fit to the style guide emphasising readability all complicated embedded logic involving pointers, complex array maniputations etc. __must__ be abstracted into libraries. 
These libraries may be maintained on a per launch repository level, or more generalised libraries may be contained in their own repository within the organisation.

## Function/Library Naming Conventions
Functions used internally within libraries do not need to follow extremely discriptive naming conventions, but libraries should be named such that public functions being called on them are easily human readable.
An example of a sufficiently descriprive function:

__Do:__ `radio.sendData(String);`

__Dont:__ `RFM22B.writeBytes(char *);`

All conversion of values from easily understandable types such as `String`, to more usable types like `char[]` must be done internally within the library to avoid pointers.

## Variable Naming Conventions
Descriptive variable names are required within the main sketch. Verbosity is not needed, but the name of the variable must be such that the reader can discern the use of it:

__Do:__ `float accel_x;`   - Shows clearly this variable is related to the accelerometer x value

__Dont:__ `float acx;`   - Not descriptive enough

__Dont:__ `float accelerometer_x_reading;`   - Too verbose


Variables maintained internally within libraries created for this project must conform to these conventions, but also begin with an underscore to indicate private use.

If migration away from the Ardruino code style is needed in future, style guides relating to other languages will be added here.
