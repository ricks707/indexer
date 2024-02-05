# indexer
Program that allows a single axis rotary table to be used on a cnc mill via the 'index' and 'index complete' signals

Several indexer programs are hosted here and are very popular. However, this indexer program builds on the same theme but follows the G code norm for programming and allows interfacing with an existing CNC control that has the ability to generate an 'Index Now' command, and when completed, generate an 'Index Complete' signal. Provisions are made for use of stepper motors or servo motors.

In the CNC world, the axis are defined as follows:
X axis is the primary linear axis as defined by a standard number line
Y axis is the primary linear axis perpendicular to the X axis on a standard number line
Z axis is the primary lenear axis perpendicular to both the X and Y axis on a standard number line, generally the height off of a milling machine table, or the rotary axis on a lathe.
A axis is the first rotary axis, that can be defined in several different ways depending on how you attach the rotary axis to your milling machine
B axis is an additional rotary axis that I have not ever used.
C axis is the second rotary axis that is typically at right angle to the A axis

G code Commands
G02 clockwise movement
G03 counterlockwise movement
G04 dwell (delay timer)
G90 absolute angular position
G91 incremental angular position
G92 circular division
G22 Program Block
G99 End of Program Block

M codes
M79 Index complete
M12 index command


