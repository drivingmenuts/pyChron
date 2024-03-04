# pyChrono

A library for timing python script execution.

### Chronograph

Works like an individual stopwatch.

You can:

* start the chronograph
* stop the chronograph
* check to see if it's running
* check the elapsed time
* set a mark
* get a list of msrks
* reset the chronograph

### Timers

A class for creating a bank of Chronographs (eg., for timing multiple events during script execution, each with its own
Chronograph). By default, a timer labeled `_internal` is created, which is useful for tracking the overall runtime of a
script.

In addition to the standard functions for any Chronograph, ou can:

* add a Timer(a Chronograph)
* get a list of Timers

By default, a Chronogrsph is accurate to 5 decimal places, which can be changed by setting `CHRONO_DEFAULT_PRECISION` to
a different value. Behind the scenes, it used the Decimal library to enable a fixed precision.


