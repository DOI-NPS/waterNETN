# waterNETN
This package contains functions that import database views from the water data package Access database and or 
CSVs in the NETN water data package and provides functions to query, summarize, and visualize NETN water data.
The R package can be installed using `pak::pkg_install('doi-nps/waterNETN')`. Previous archived 
versions of this R package can be found at <a href="www.github.com/katemmiller/waterNETN">
www.github.com/katemmiller/waterNETN</a>

This package includes the following functions: 
<ul>
<li>importData: Import views from data package MS Access database or as a zip file of csvs.</li>           
<li>exportData: Export views as CSVs to prepare for data package.</li>
<li>prepFMtoAccess: preps water data exported from the FileMaker app for import into the MS Access backend database. 
Note: Not sure if this function is fully functional (depends on whether database is set up to import a CSV).</li>  
<br>
<li>getSites: queries location information common across lakes and streams.</li>
<li>getSitesLake: queries location information specific to lakes.</li>
<li>getSitesStream: queries location information specific to streams.</li>
<li>getEvents: queries visit-level data for NETN water monitoring.</li>
<br>
<li>getChemistry: queries NETN water chemistry data that were measured in the lab.</li>
<li>getDischarge: queries NETN water discharge data for stream sites.</li>
<li>getLightPen: queries light penetration data for lake monitoring.</li>
<li>getSecchi: queries Secchi depth data for lake monitoring.</li>
<li>getSondeInSitu: queries water data collected with by a Sonde in the field.</li>
<li>getStreamObs: queries stream observation data.</li>
<li>getWaterLevel: queries water level data.</li> 
<br<
<li>plotLakeProfile: plots metrics collected in lake profiles.</li>     
<li>plotPrecipDischarge: plots precipitation vs. stream discharge. The package doi-nps/climateNETN must be installed for this function. </li> 
<li>plotScatterPlot: plots a scatterplot of 2 water quality or quantity metrics.</li>    
<li>plotTrend: plots a water metric over time and includes option to add loess smoother.</li>           
<li>plotWaterBands: plots current year of water in comparison to the distribution of water data collected in specified previous years.</li>      
<br>
<li>theme_WQ: custom ggplot2 theme for plotting NETN water data.</li>  
</ul>

The docs/ folder includes multiple files that are useful for automated reporting and the tutorial website: 
<ul>
<li>index.Rmd and its output index.html are the files that generate the <a href = "doi-nps.github.io/waterNETN">
waterNETN tutorial website</a>. </li> 
<li>QC_NETN_report.RMD performs automated QC checks on the data. Note that the WC_NETN_compile.R and QC_NETN_report_functions.R 
are sourced in the RMD.</li>
<li>header_manual.html generates th NPS banner for both RMD headers.</li>
<li>www/ folder contains the css and images sourced in the RMDs.</li>
</ul>


