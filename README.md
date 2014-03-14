chl
===

CHangeLogger

chl is a little PERL script, used to record a change or to display changes performed on one or more servers or devices defined in a MySQL DB
The filtering method is inspired from MCollective:

-I /regexp/

(I => Identity) for filtering device name based on the regular expression


-F db_field=db_value

(F => Field) only device matching specfied db_value for db_field


example of my db_fields : environment, is_virtual, serverroom, osversion, ...


this script filters first on db_fields. If many of them, the relation is AND
then on Identites. If many of them, the relation is OR
