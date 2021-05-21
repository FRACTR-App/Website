# FRACTR Website

Files for the Fire Resource Area Coverage Time to Response (FRACTR) project website.

### Public GeoJson Data

The code that generates all data below is located in the project's main [FRACTR repository](https://github.com/This-blank-Is-On-Fire/FRACTR).

The [data folder](https://github.com/This-blank-Is-On-Fire/Website/tree/master/data) contains all geoJson files displayed to the website.
 - Fire station coordinates (`fire_station_coords.geojson`)
 - State-defined Emergency Service Zones (`zone_polygons.geojson`)
 - State-defined Fire Department Emergency Service Zones (`dissolved_zones.geojson`)
 - Vermont state boundaries (`vermont_state_polygon.geojson`)
 - Response time polygons, where network analysis is bounded by the entire state (e.g., `2.geojson` contains all polygons displaying 2-minute reach from stations)
 - Response time polygons, where network analysis is bounded by state-defined Emergency Service Zones, aka ESNs (e.g., `2_esn.geojson`)
 - Hydrant locations surrounded by circle polygons of radius = 600 feet, color-coded by flowrate (e.g., `hydrant_red.geojson` contains circle polygons of hydrants with flowrate less than 500 gallons per minute – see [this NFPA page](https://www.soteriafiresa.com/fire-hydrant-colours/) for hydrant flowrates & types)

All data above has been collected from the [Vermont Open Geodata Portal](https://geodata.vermont.gov/), which we are thoroughly grateful for.

### Ethical Implications of our work
These maps offer rough estimates of response times and should not be interpreted as exact, reliable fact. Fire station response protocols vary and may impact response times. Differences in fire station resources are not taken into account. 
Additionally, future homeowners and insurance companies might use our application 
as a tool to discriminate between properties located near and far away from fire stations. Consequently, future homeowners may be less likely to purchase homes located outside of certain response time zones, and insurance companies could choose to raise insurance costs for homes in these areas. We recognize these possibilities and remind our users that these maps offer estimates and should be used for public governance, citizen awareness, and emergency planning. Our hope is that regional planning commissions and state emergency planners can use these maps to inform their 
work and increase coverage across the state. If you have any issues with these maps, 
please reach out to us at jcambefort@middlebury and halcyonb@middlebury.edu, as we would be happy to hear your thoughts. 