[Back to Index](/Documents/Protocol/index.md)

Position Message
================

- Protocol Version: 3.0
- Release Date: January 20, 2017


Summary
===================

The POSITION data type is used to transfer position and orientation information. The data are a combination of 3-dimensional vector for the position and quaternion for the orientation. Although equivalent position and orientation can be described with the TRANSFORM data type, the POSITION data type has the advantage of smaller data size (19%). It is therefore more suitable for pushing high frame-rate data from tracking devices.

Message Types
===================

POSITION
-------------------

<table border="1" cellpadding="5" cellspacing="0" align="center">
<tr>
<td style="background:#e0e0e0;"> Data
</td><td style="background:#e0e0e0;"> Type
</td><td style="background:#e0e0e0;"> Description
</td></tr>
<tr>
<td align="left"> X
</td><td align="left"> 32-bit float
</td><td align="left"> X position in millimeter
</td></tr>
<tr>
<td align="left"> Y
</td><td align="left"> 32-bit float
</td><td align="left"> Y position in millimeter
</td></tr>
<tr>
<td align="left"> Z
</td><td align="left"> 32-bit float
</td><td align="left"> Z position in millimeter
</td></tr>
<tr>
<td align="left"> OX
</td><td align="left"> 32-bit float
</td><td align="left"> X element in quaternion
</td></tr>
<tr>
<td align="left"> OY
</td><td align="left"> 32-bit float
</td><td align="left"> Y element in quaternion
</td></tr>
<tr>
<td align="left"> OZ
</td><td align="left"> 32-bit float
</td><td align="left"> Z element in quaternion
</td></tr>
<tr>
<td align="left"> W
</td><td align="left"> 32-bit float
</td><td align="left"> W element in quaternion
</td></tr>
</table>

GET_POSITION
-------------------

<table border="1" cellpadding="5" cellspacing="0" align="center">
<tr>
<td style="background:#e0e0e0;"> Data
</td><td style="background:#e0e0e0;"> Type
</td><td style="background:#e0e0e0;"> Description
</td></tr>
</table>

STT_POSITION
-------------------

<table border="1" cellpadding="5" cellspacing="0" align="center">
<tr>
<td style="background:#e0e0e0;"> Data
</td><td style="background:#e0e0e0;"> Type
</td><td style="background:#e0e0e0;"> Description
</td></tr>
</table>

STP_POSITION
-------------------

<table border="1" cellpadding="5" cellspacing="0" align="center">
<tr>
<td style="background:#e0e0e0;"> Data
</td><td style="background:#e0e0e0;"> Type
</td><td style="background:#e0e0e0;"> Description
</td></tr>
</table>

RTS_POSITION
-------------------

<table border="1" cellpadding="5" cellspacing="0" align="center">
<tr>
<td style="background:#e0e0e0;"> Data
</td><td style="background:#e0e0e0;"> Type
</td><td style="background:#e0e0e0;"> Description
</td></tr>
<tr>
<td align="left"> Status
</td><td align="left"> 8 bit unsigned
</td><td align="left"> 0: Success 1: Error
</td></tr>
</table>

Implementations
===================

POSITION type is implemented in the following files:
* [igtlPositionMessage.h](/Source/igtlPositionMessage.h)
* [igtlPositionMessage.cxx](/Source/igtlPositionMessage.cxx)

Contributors
===================

* Junichi Tokuda