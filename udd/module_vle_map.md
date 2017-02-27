# module_VLE_map

*  [MODULE_VLE_MAP_ID](#module_vle_map_id) [1] **
*  [MOD_INSTANCE_ID](module_instance.md#mod_instance_id) [1] *
*  [VLE_MOD_ID](#vle_mod_id) [1] *

\** indicates that the property is the primary key for this entity.  
\* indicates that the property is part of a uniqueness constraint for this entity.

##Description of module_VLE_map entity
A module_VLE_map links a module in a student record system with module materials in a VLE.

##MODULE_VLE_MAP_ID
###Description
UDD generated identifier for map between module and VLE. 

###Purpose
Enables easy reference to the map between module and VLE.

###Derivation
Jisc

###Format
UDD generated.  Do not include when supplying data.
String(255)

###Notes
UDD generated.  Do not include when supplying data.


##VLE_MOD_ID
###Description
An unique identifier for a course area in the VLE. 

###Purpose
Display in student app and staff dashboard

###Derivation
Jisc

###Valid values
Any

###References

###Format
String(255)

###Notes
The VLE course area may or may not correspond to one module.
