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

### Limitations of the Maps & Data
 - These maps offer rough estimates of response times and should not be interpreted as exact, reliable fact (the road network and speed data are fetched from openstreetmap.org).
 - Fire station response protocols vary and may impact response times.
 - Differences in fire station resources are not taken into account.
 - Any stations missing on the map were either missing in the original dataset, or misleadingly labeled (e.g., labeled strictly as a law enforcement station).
- To compute a station's response polygons, a mapping is created between the fire station coordinates and the nearest node on the Open Street Maps network graph.
However, occasionally, the nearest node on the graph may be a few hundred feet away from the station and thus the polygon produced is slightly off-centered.


### Ethical Implications of Our Work

These maps offer rough estimates of response times and should not be interpreted as exact (see the Limitations section).
A concern of ours is that future homeowners and insurance companies may seek to use our maps as a tool to discriminate between properties located near and far away from fire stations. Consequently, future homeowners may be less likely to purchase homes located outside of certain response time zones, and insurance companies could choose to raise insurance costs for homes in 
these areas. We recognize these possibilities and remind our users that these maps offer estimates and should be used for public governance, citizen awareness, and emergency planning. Our hope is that regional planning commissions and state emergency planners can use these maps to inform their work and increase coverage across the state.

If you have any issues with these maps, please reach out to us at [jcambefort@middlebury.edu](mailto:jcambefort@middlebury.edu) and [halcyonb@middlebury.edu](mailto:halcyonb@middlebury.edu), as we would be happy to hear your thoughts.


### Acknowledgments

Thank you to Middlebury Fire Department Chief David Shaw and Andrew L'Roe at the Addison County Regional Planning Commission for their input on local datasets and the Vermont fire service, and for troubleshooting our website. Thank you very much to Bill Hegman, Prof. Holler, Prof. Kimambo, and Kufre Udoh from the Middlebury College Geography Department for their insights into network analysis and working with raster and vector data. Thank you to Prof. Vaccari for overseeing the Computer Science Senior Seminar course and guiding us through this process.