3-30-300 Urban Tree Optimization Model Based on a Set-Cover Algorithm

Description

This repository contains the implementation of a spatial Set-Cover optimization model developed to support the operationalization of the 3-30-300 urban nature rule at the parcel scale. The objective of the model is to identify the minimum number of new trees required to ensure that each residential parcel has visibility to at least three trees within a 30-meter radius. The approach prioritizes planting locations along social and green corridors in order to enhance proximity to nature, support equitable urban greening, and improve environmental quality in dense urban environments.

Method Summary
The methodology involves the generation of candidate tree-planting points along designated walkable or green corridors at regular spatial intervals. Each candidate location is buffered to simulate a tree’s visibility radius. A spatial intersection procedure is then carried out to determine which residential parcels fall within each buffer area. A greedy Set-Cover algorithm subsequently selects locations that offer the highest marginal contribution to unsatisfied parcels until the minimum visibility threshold for each parcel is achieved.

Requirements
The model requires ArcGIS Pro with arcpy and a file geodatabase containing residential parcels and social/green corridors. The tool is designed for Python 3.9–3.11, corresponding to the ArcGIS Pro Python environment. No data are provided in this repository due to licensing restrictions.


The output is a feature class containing the optimized tree locations that satisfy the model’s objective. Summary metrics are printed in the console, including number of selected trees, parcel satisfaction rate, and coverage efficiency.


Licensing

This repository is released under the MIT License, permitting reuse and modification with appropriate attribution.
