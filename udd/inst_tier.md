#inst_tier
* [INST_TIER_ID](#inst_tier_id) [1] *
* [INST_TIER_NAME](#inst_tier_name) [1]

\* indicates that the property is the primary key for this entity.

###Description
An inst_tier is an organisational sub-unit of an institution. This entity simply identifies and names the organisational sub-unit; it does not attempt to model institutional structures.


##INST_TIER_ID
###Description
The institution's identifier or code for the organisational sub-unit.

###Purpose
To enable look-up of the name of the organisational sub-unit for labelling within a dashboard or other interface.

###Derivation
Institution

###Valid Values
Any

###Format
String (255)

###Notes

##INST_TIER_NAME
###Description
The official title of the organisational sub-unit.

###Purpose
To provide a locally recognisable label within a dashboard or other interface.

###Derivation
Institution

###Valid Values
Any

###Format
String (255)

###Notes
Examples: "Faculty of Arts", "School of History and Philosophy", "Department of Ancient History"
