# Requesting Hazard Types

To request the list of hazard types configured in the system please use the route defined here:

[https://enterprise.disasteraware.com/hp\_srv/\#!/hazards/getHazard\_TypesTokenServer\_JSON](https://enterprise.disasteraware.com/hp_srv/)

This request will return an array that contains all of the hazard types.  Each element in the array will have three properties:

1. **type\_id** - This is like the primary key for the hazard type.  This is the value that will be found on the hazard object.
2. **type\_name** - A human readable value for the hazard e.g. Volcano
3. **type\_icon** - This is the url for the hazard type icon’s image e.g. avalanche.png. The hazard icons are hosted at:[ https://static.pdc.org/icons/hazard/large/](https://static.pdc.org/icons/hazard/large/).  To construct the fully qualified location for the hazard type’s icon combine the host location with type\_icon value.



