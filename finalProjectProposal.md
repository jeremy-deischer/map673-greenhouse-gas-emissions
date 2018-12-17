## Final Project Proposal

For the final project for MAP 673 I'm interested in exploring how proposed stream
improvements change over time and how those improvements are implemented.  More
specifically, I will explore improvements from Urban Drainage and Flood Control
District (UDFCD) Major Drainageway Plans (MDP) and Outfall System Plans (OSP).  
UDFCD teams with local jurisdictions to study local drainageways and develop proposed
improvements to be constructed as funding becomes available.  

The data for the map will be obtained from [Open Data Colorado](http://data.opencolorado.org/dataset?q=udfcd).
Available datasets include both base data (watersheds, streams, UDFCD boundary)
as well as improvements proposed in both MDP and OSP studies.

The main objective for the map will be to look at the spatial and temporal distribution of proposed improvements.  
The map will allow the user to view how proposed improvements change throughout time and where studies have been developed.  
The target audience would be participants at local jurisdictions interested in improvements along their local drainageways.  
For example, John at Jefferson County would be interested in seeing how the proposed improvements in streams in Jefferson County change from the last few years.  
He would be able to view what streams have been studied the type of improvements that have been recommended.

The webmap will show the different kind of proposed improvements along each drainageway.  Proposed improvements from each study
has been digitized with information on the type of improvements.  Based on what trends are observed as the data is examined,
the anticipated thematic representation would be a cloropleth of the percentage of projects built along each stream or total
dollars invested. Each type of improvements will be represented by a different type of symbol. The user will be able to filter
by a specific watershed with a slide control to sequence through the dataset. The map will also be able to reexpress based on
the type of improvement and retrieve further information with a tooltip.

The anticipated user interaction consists of filtering the type of proposed improvement and filtering by watershed.  Type of improvement
will be controlled by buttons while watershed filter will have a dropdown.  Year of improvement will be controlled by a slider grouped
by 5 years or each decade.  

#### Anticipated Technology Stack:
+ Data Format:

   The data will be stored in a GeoJSON format.

+ Data Processing:

   The majority of the data processing will be completed in QGIS.  Slight processing is expected of assigning which stream improvements are located on by spatial query and extracted the date of studies from a field that includes the full length of the project name.

+ Other relevant technologies:

   Several different web technologies will be employed while developing the webmap.  The most significant technologies that will be utilized include HTML, CSS, and Javascript.  The main Javascript libraries that will be used include Leaflet and D3.

+ Hosting Platform:

   Github pages will be used to host the webmap.
