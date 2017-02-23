#Extension
This section does not form a part of the formal UDD specification.

##Description
There is provision here for data extensions at the level of property (in other words, "field-level extensions").  The purpose of this is to enable institutions and vendors to experiment with new or proprietary properties in any UDD entity that may be relevant only to one or a few institutions, and may be specific to a vendor.  For example, an institution may wish to introduce a flag on student to indicate that a student was a member of an institution's sports team.

The records in the extension entity consist of 5 parts, described here.  The purpose of the record is to identify the vendor or institution that is using this extension, the entity involved, the specific record that is extended, the name of the extension property and its value.  For example (using a CSV format):

```
Tribal, student, ST123456, SPORTS_TEAM_FLAG, Y
```

* [VENDOR](#vendor) [1] *
* [ENTITY](#entity) [1] *
* [PRIMARY_KEY](#primary_key) [1] *
* [PROPERTY_NAME](#property_name) [1] *
* [PROPERTY_VALUE](#property_value) [1]

##VENDOR
###Description
Identifies the vendor to which this extension applies.

###Valid Values
Standard list of vendor identifiers to be used.

###Purpose
Enables identification of a group of extensions by vendor.

###Format
String (255)

###Notes

##ENTITY
###Description
Names the UDD entity extended by this record.

###Purpose
Identifies the relevant entity.

###Valid Values
<table>
	<tr>
		<td>ENTITY</td>
	</tr>
	<tr>
		<td>assessment_instance</td>
	</tr>
	<tr>
		<td>course</td>
	</tr>
	<tr>
		<td>course_instance</td>
	</tr>
	<tr>
		<td>institution</td>
	</tr>
	<tr>
		<td>module</td>
	</tr>
	<tr>
		<td>module_instance</td>
	</tr>
	<tr>
		<td>module_vle_map</td>
	</tr>
	<tr>
		<td>period</td>
	</tr>
	<tr>
		<td>staff</td>
	</tr>
	<tr>
		<td>staff_on_course_instance</td>
	</tr>
	<tr>
		<td>staff_on_mod_instance</td>
	</tr>
	<tr>
		<td>student</td>
	</tr>
	<tr>
		<td>student_course_membership</td>
	</tr>
	<tr>
		<td>student_on_a_module_instance</td>
	</tr>
	<tr>
		<td>student_on_assessment_instance</td>
	</tr>
	<tr>
		<td>student_on_course_instance</td>
	</tr>
</table>

###Format
String (255)

###Notes

##PRIMARY_KEY
###Description
Holds the unique single primary key identifying the record to which the extension applies.

###Purpose
Identifies the relevant extended record.

###Valid Values
Any

###Format
String (255)

###Notes
Must use the single primary key, not a composite key.


##PROPERTY_NAME
###Description
Label for the extension.

###Purpose
Identifies the extension used.

###Valid Values
Label drawn from a vocabulary of valid labels for extensions.

###Format
String (255)

###Notes


##PROPERTY_VALUE
###Description
Data held against the extension for the specific record identified by the ENTITY and PRIMARY_KEY.

###Purpose
Holds the extended data.

###Valid Values
Any

###Format
Any

###Notes


