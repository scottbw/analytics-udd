#Period
* [MOD_PERIOD](#mod_period) [1] *
* [ACADEMIC_YEAR](#academic_year) [1] *
* [PERIOD_START_DATE](#period_start_date) [1]
* [PERIOD_END_DATE](#period_end_date) [1]

\* indicates that the property is the primary key for this entity.

###Description
A period describes a provider's official start date and end date of time slices, such as academic years, terms and semesters that are used in the UDD data.  For the dates of an academic year, the MOD_PERIOD uses the fixed string "Academic Year".  For other periods, MOD_PERIOD uses institution-defined string values in conjunction with the 4-digit value of the ACADEMIC_YEAR property to record the start and end dates of the specified periods.

##MOD_PERIOD
###Description
The provider's own unique label for the period (e.g. semester 1)

###Purpose
To enable identification of the time period using the institution's terminology.

###Derivation
Institution

###Valid Values
Where this record sets the dates for the institution's academic year, MOD_PERIOD should be set to "Academic Year".
Otherwise any.

###Format
String (255)

###Notes
Examples: "semester 1", "Spring term".


##ACADEMIC_YEAR
###Description
The year in which the beginning of the relevant academic year starts.

###Purpose
For display and analysis purposes

###Derivation
Jisc

###Valid Values
Year in ISO 8601 format - YYYY; ie year that the academic year starts in.

###Format
String in ISO 8601 Year format - YYYY

###Notes


##PERIOD_START_DATE
###Description
Official start date for this period

###Purpose
For display and analysis purposes

###Derivation


###Valid Value
Date in ISO 8601 format - YYYY-MM-DD


###References


###Format
String in ISO 8601 Date extended format - YYYY-MM-DD

###Notes


##PERIOD_END_DATE
###Description
Official end date for this period

###Purpose
For display and analysis purposes

###Derivation


###Valid Values
Date in ISO 8601 format - YYYY-MM-DD

###References


###Format
String in ISO 8601 Date extended format - YYYY-MM-DD

###Notes

