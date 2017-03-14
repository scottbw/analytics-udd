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
Values should be one of the following:
HUSID
ULN
a URL that identifies the system within which IDENTIFIER exists, for example a VLE

###Format
String(255)

###Notes


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


