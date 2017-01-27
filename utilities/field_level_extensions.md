#Field level extensions

Institutions and vendors may wish to extend the UDD data fields for specific purposes that do not apply to other institutions or vendors.  Rather than extend the UDD properties for standardised UDD entities, this type of data can be loaded into the LRW using the following JSON structure.

?This data would not be validated through normal UDD validation routines, as it is JSON format data.  What validation applies, if any?

The structure contains:

* the UDD entity for which the data field is an extension.
* the vendor (or institution if using own software) to which the data relates.

##Description of field level extension structure

The data must be in the following JSON format:

?Is the UDD entity name from the md file OK for this?

AAAAAA
bbbbbb: { // any data here
	bbbbbbext1: "cccccc",
	bbbbbbext2: "dddddd"
}

where
- AAAAAA is the UDD entity name exactly as stated in the UDD MD file.
- bbbbbb is the vendor's name (or institution if using own software).  This name should be a single unique string for each vendor.
- bbbbbbext1 is the field name for the first extension.
- cccccc is the data value in the first extension field.
- bbbbbbext2 is the field name for the second extension.
- dddddd is the data value in the second extension field.

##Example

STUDENT_ID,
tribal: { // test data for eye and hair colour
  eye_colour: "brown",
  hair_colour: "brown"
}

?could we have a realistic example please?

##Control

Existing UDD field names from any UDD entity must not be used.
It is the responsibility of the vendor (or institution) to ensure that there are no clashes of field names within the domain of the institution to which the extension applies.
