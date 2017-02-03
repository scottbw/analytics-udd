#course_location
* [COURSE_LOCATION_ID](#course_location_id) [1] *
* [COURSE_LOCATION_NAME](#course_location_name) [1]

\* indicates that the property is the primary key for this entity.

###Description
A course_location is a campus or other location that indicates where a student is studying on a course_instance (see student_on_course_instance). This entity simply identifies and names the location; it does not give further geographical information.


##COURSE_LOCATION_ID
###Description
The institution's identifier or code for the location.

###Purpose
To enable look-up of the name of the location for labelling within a dashboard or other interface.

###Derivation
Institution

###Valid Values
Any

###Format
String (255)

###Notes

##COURSE_LOCATION_NAME
###Description
The official title of the location.

###Purpose
To provide a locally recognisable label within a dashboard or other interface.

###Derivation
Institution

###Valid Values
Any

###Format
String (255)

###Notes
Examples: "Main Campus", "Park Campus", "Centre for Performing Arts"
