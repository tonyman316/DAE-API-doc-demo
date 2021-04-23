# What are Global Active Hazards?

A hazard is an incident e.g. earthquake, volcano, tornado etc… that has reached a threshold where it has become a significant danger to life and property.  DAE’s DaaS provides global hazard information.  Hazard as a data object has three main definitions:  


1. **Type** — This property defines what kind of hazard is it.  Examples of hazard type include: Earthquakes, Wildfires, Tropical Storms etc… etc… Each hazard type has a set of associated data layers that help put the hazard into context.  For example, the United States Geological Society’s Shake Map helps both users and automated processes understand the impact of an earthquake.
2. **Severity** — This value represents how dangerous is the hazard.  In order of least to most severe the possible values are: TERMINATION, INFORMATION, ADVISORY, WATCH and WARNING.
3. **Category** — Typically an on-going hazard is an event.  However, if the hazard requires a major response after the initial impact the category can be switch to a response.  The possible values for hazard category are: EVENT, EXERCISE, OTHER and RESPONSE.

When viewing a hazard in the DisasterAWARE application the symbol associated to a hazard will be a composite of these three values.  The icon in the center of the symbol is the hazard type.  The type of geometry around the icon indicates its category.  For example, events are symbolized by circles.  This is commonly referred to as the halo.  The color of the “halo” indicates its severity.  For example, WARNING level hazards have a red color halo to indicate they are the most urgent.  


