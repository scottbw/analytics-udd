# institution
* [TENANT_ID](#tenant_id) [1] **
* [TENANT_NAME](#tenant_name) [0..1]
* [UDD_VERSION](#udd_version) [1]
* [MODULE_VLE_MAP_MODE](#module_vle_map_mode) [1]

\** indicates that the property is the primary key for this entity.

## Description of institution entity
An institution is the overall provider of one or more courses.  Example: University of Gloucestershire.

## TENANT_ID
### Description
This field records the unique identifier for the University College concerned - using the UK Provider Reference Number (UKRPN) which is the unique identifier allocated to institutions by the UK Register of Learning Providers (UKRLP).

### Purpose
To identify the organisation.

### Derivation
UK Register of Learning Providers (UKRLP).

### References

### Format
String (8)

### Notes
Further information (on UKPRN) available at www.ukrlp.co.uk


## TENANT_NAME
### Description
Institution's official legal name. This should match the name indicated in the UKRLP database, as used for TENANT_ID

### Purpose
To identify the organisation.

### Derivation
Institution

### References

### Format
String (255)

### Notes
Omitting this property could impair the functionality of analytics applications such as student apps or dashboards.

## UDD_VERSION
### Description
Version number of this UDD specification.

### Purpose
Enables the UDD to be self-declaring of its version.

### Derivation
UDD specification in use by the institution

### References

### Format
String (8)

### Notes
Value will be the current version number of the UDD preceded by "v".  Example: if the data uses UDD v1.3.0, value will "v1.3.0".


## MODULE_VLE_MAP_MODE
### Description
This property prescribes for this institution how the mapping between MOD_INSTANCE_ID and VLE_MOD_ID works in the module_VLE_map entity. The modes are given in the valid values table.

### Purpose
To enable the constraints on the module_VLE_map entity to be varied between institutions.

### Derivation
Jisc

### Valid Values
<table>
<tr><td>MODULE_VLE_MAP_MODE</td><td>DESCRIPTION (ENGLISH)</td><td>DESCRIPTION (WELSH)</td></tr>
<tr><td>0</td><td>Default. 1 MOD_INSTANCE_ID value maps to 1 and only 1 VLE_MOD_ID value.</td><td></td></tr>
<tr><td>1</td><td>1 MOD_INSTANCE_ID value maps to 1 or many VLE_MOD_ID values.</td><td></td></tr>
<tr><td>2</td><td>1 VLE_MOD_ID value maps to 1 or many MOD_INSTANCE_ID values.</td><td></td></tr>
</table>

### Format
Int

### Notes
Default value is "0".