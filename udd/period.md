#Period
* [PERIOD_ID](#period_id) [1] *
* [PERIOD_TYPE](#period_type) [1]
* [PERIOD_START_DATE](#period_start_date) [1]
* [PERIOD_END_DATE](#period_end_date) [1]
* [TENANT_ID](institution.md#tenant_id) [0..1]

\* indicates that the property is the primary key for this entity.

###Description
A period describes a provider's official start date and end date of time slices, such as academic years, terms and semesters that are used in the UDD data.

##PERIOD_ID
###Description
The provider's own label for the period.

###Purpose
To identify the period record.

###Derivation


###Valid Values
Any

###Format
String (255)

###Notes
Examples: "semester 1, 2017", "2017-18 Academic Year".


##PERIOD_TYPE
###Description
Controlled text description for the time slice, for example ACADEMIC_YEAR, MOD_PERIOD.  Must match the property name in the UDD entity to which it refers.

###Purpose
To enable identification of the time slice in UDD context.

###Derivation


###Valid Values
<table>
            <tr>
                <td>PERIOD_TYPE</td>
            </tr>
            <tr>
                <td>ACADEMIC_YEAR</td>
            </tr>
            <tr>
                <td>MOD_PERIOD</td>
            </tr>
            <tr>
                <td>TERM</td>
            </tr>
            <tr>
                <td>SEMESTER</td>
            </tr>
</table> 

###Format
String (255)

###Notes
Could be extended to include other periods as required.


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

