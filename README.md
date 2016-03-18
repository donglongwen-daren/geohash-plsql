# geohash-plsql

## Oracle PL/SQL GeoHash Encoder Implementation


### Overview
An implementation of the GeoHash encoder for Oracle PL/SQL based on the the work of

+ https://github.com/sharonjl/geohash-net
+ https://github.com/davetroy/geohash-js

### Usage
GEOHASH_ENCODE( LATITUDE, LONGITUDE, PRECISION )

### Usage
Parameters
+ LATITUDE : Floating point
+ LONGITUDE : Floating point
+ PRECISION : Optional integer (default: 5)

### Return Value
A varchar2 having a length of the specified precision.

### Example
`SQL> select GEOHASH_ENCODE( 32.775833, -96.796667 ) GEOHASH from dual;`  
`GEOHASH`  
`---------`  
`9vg4m`  
