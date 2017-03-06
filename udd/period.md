#period

* [PERIOD_ID](#period_id) [1] **
* [PERIOD_CODE](#period_code) [1] *
* [ACADEMIC_YEAR](#academic_year) [1] *
* [PERIOD_NAME](#period_name) [1]
* [PERIOD_START_DATE](#period_start_date) [1]
* [PERIOD_END_DATE](#period_end_date) [1]

\** indicates that the property is the primary key for this entity.
\* indicates that the property is part of a uniqueness constraint for this entity.

##Description
A period describes an institution's official start date and end date of time slices, such as academic years, terms and semesters.

##PERIOD_ID
###Description
Primary key. Where not supplied by data provider, the primary key will be UDD generated.

###Purpose
Enables easy reference to period.

###Derivation
Jisc

###Format
Concatenation of PERIOD_CODE and ACADEMIC_YEAR, separated by a tilde (~).
String(255)

###Notes
Where not supplied by data provider, the primary key will be UDD generated.



##PERIOD_CODE
###Description
The institution's own code for the period.

###Purpose
To enable identification of the time period using the institution's own code, unique in any 1 academic year.

###Derivation
Institution

###Valid Values
Where the period record states the dates for the institution's academic year, PERIOD_CODE must use the fixed string "ACADYR". For other periods, PERIOD_CODE uses institution-defined code values. Each different code value in module_instance.MOD_PERIOD must have a matching code value in PERIOD_CODE. Where the same code values are used across different academic years, the specific period record can be identified by reference to the PERIOD_CODE together with the ACADEMIC_YEAR property; these properties together form the primary key.

###Format
String (255)

###Notes
Examples: "SEM1", "WHOLE YEAR", "TRMS1+2"


##ACADEMIC_YEAR
###Description
The year in which the start of the relevant academic year happens.

###Purpose
For lookup and analysis purposes.

###Derivation
Jisc

###Valid Values
Year in ISO 8601 format - YYYY; ie year that the academic year starts in.

###Format
String in ISO 8601 Year format - YYYY

###Notes


##PERIOD_NAME
###Description
The institution's own human readable label for the period (e.g. "Spring Term, AY 2016-17").

###Purpose
To display the time period using the institution's terminology.

###Derivation
Institution

###Valid Values
Any.

###Format
String (255)

###Notes
This value is intended to display the period, so that a human reader can understand it.  For clarity the relevant academic year should be included, as in this example: "Semester 2, AY 2016/17".


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

