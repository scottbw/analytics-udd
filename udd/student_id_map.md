#student_id_map
* [STUDENT_ID](student.md#udd_student_id) [1] *
* [DOMAIN](#domain) [1] *
* [IDENTIFIER](#identifier) [1] *

\* indicates that the property is part of a composite primary key for this entity.

##Description
The UDD student identifier entity enables efficient processing of IDs in relation to both the UDD structures and xAPI statements.

##DOMAIN
###Description
Identifies the system within which IDENTIFIER exists.

###Purpose
Efficient processing of IDs, and lookup of data in xAPI statements.

###Valid values
<table>
	<tr>
		<td>DOMAIN</td>
	</tr>
	<tr>
		<td>HUSID</td>
	</tr>
	<tr>
		<td>ULN</td>
	</tr>
	<tr>
		<td>VLE_1</td>
	</tr>
	<tr>
		<td>VLE_2</td>
	</tr>
	<tr>
		<td>VLE_3</td>
	</tr>
</table>

###Format
String(255)

###Notes
The value of IDENTIFIER where DOMAIN value = "VLE_1" is the VLE_ID in the student entity; "VLE_1" is the main VLE. 


##IDENTIFIER
###Description
Local ID for the student, as used in DOMAIN.

###Purpose
Enables identification of student in DOMAIN.

###Valid values
Any

###References

###Format
String (255)

###Notes


