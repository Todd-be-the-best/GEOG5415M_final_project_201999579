# GEOG5415M_final_project_201999579
GEOG5415M_final_project

# **Exploring ULEZ post-expansion air quality patterns across central and outer London**

Student ID number: 201999579


## **Background and Literature**

Air pollution is a major environmental risk to human health in large metropolitan areas. In London, nitrogen dioxide (NO₂) and particulate matter (PM) remain key pollutants, with long-term exposure linked to respiratory and cardiovascular disease, reduced life expectancy, and broader societal costs. Although air quality has improved across the United Kingdom, traffic-related pollutant concentrations in London frequently exceed recommended guideline levels, particularly at roadside and central locations.

Road transport is a dominant source of urban air pollution in London. Policies such as the Low Emission Zone (LEZ) and Ultra Low Emission Zone (ULEZ) have been introduced to reduce vehicle emissions, but evidence suggests their effects are limited and spatially heterogeneous. Using causal inference methods, Ma et al. (2021) find that the introduction of the central London ULEZ in 2019 led to only modest reductions in NO₂ relative to long-term trends, with no statistically significant effects on PM₂.₅. Consistent with this, Tong et al. (2025) show that while early ULEZ phases reduced roadside NO₂ in central London, subsequent expansions produced little additional benefit for NO₂ and no significant improvement in PM₂.₅.

Recent research highlights the importance of fine-scale spatio-temporal analysis. High time-resolution roadside monitoring in central London reveals substantial short-term variability in NO₂ concentrations, driven by traffic intensity, atmospheric chemistry and local meteorological conditions (Campbell et al., 2024). Moreover, air pollution has been shown to affect human well-being. Higher NO₂ concentrations are associated with lower life satisfaction (MacKerron et al., 2009), while air quality improvements following LEZ and ULEZ implementation are linked to reduced sick leave and improved mental well-being (Beshir et al., 2025). Together, these findings underline the value of analysing spatial and temporal variation in air pollution across central and suburban environments.


## **Data**

This project uses openly available air quality and spatial data to examine post-expansion air quality patterns across central and outer London.

### **Air quality data**

Air quality measurements were obtained from the [London Air Quality](https://www.londonair.org.uk/london/asp/datadownload.asp). The analysis focuses on hourly nitrogen dioxide (NO₂) concentration data from two monitoring sites:

Regent Street (The Crown Estate): a central London roadside monitoring site representing a high-traffic urban environment.

Bexley (Belvedere): an outer London suburban monitoring site representing a lower-traffic setting.

Both datasets cover the period from 29 August 2023 to 31 December 2025, corresponding to the post-expansion phase of the London wide Ultra Low Emission Zone (ULEZ). The datasets include pollutant species, measurement timestamps and concentration values.

### **Spatial data**

Spatial boundary data for the London wide ULEZ were sourced from the [London Datastore](https://data.london.gov.uk/dataset/london-wide-ultra-low-emission-zone-2023-vd455). The ULEZ boundary dataset provides polygon geometry representing the policy coverage area following its expansion across all London boroughs on 29 August 2023.

### **Data use and scope**

The air quality data are used to compare NO₂ concentration patterns between central and outer London locations, while the spatial data provide geographical context for the monitoring sites. All data used in this project are openly access and suitable for reproducible spatial data science analysis.


## **Code objectives**

The code provides a reproducible workflow for analysing post-expansion air quality in London. It loads openly access air quality and spatial data. It cleans and prepares NO₂ measurements for analysis. Exploratory visualisations are used to support data cleaning decisions. A simple statistical model is fitted to examine differences between central and outer London sites. Final non-spatial and spatial visualisations are produced to communicate the results clearly.


## **Reproducing the analysis**

All data required to reproduce this analysis are included in the project repository. This includes the Jupyter notebook, the air quality CSV files for Regent Street (The Crown Estate) and Bexley (Belvedere), and the spatial boundary file for the London wide ULEZ. The analysis is written in Python and can be run using standard scientific Python libraries such as pandas, geopandas, matplotlib, and statsmodels. To reproduce the results, open the Jupyter notebook and run the cells in order from top to bottom. No additional data downloads or manual preprocessing steps are required.


## **References**

Beshir, H.A. and Fichera, E. 2025. 'And Breathe Normally: Impacts of low emission zones on sick leave and mental well-being', *Journal of economic behavior & organization*, June 2025. [Online]. [Accessed: 22 January 2026]. Available from: https://leeds.primo.exlibrisgroup.com/discovery/fulldisplay?docid=cdi_crossref_primary_10_1016_j_jebo_2025_106994&context=PC&vid=44LEE_INST:VU1&lang=en&search_scope=My_Inst_CI_not_ebsco&adaptor=Primo%20Central&tab=AlmostEverything&query=any,contains,london%20air%20quality&facet=searchcreationdate,include,2023%7C,%7C2026&offset=40

Campbell, S.J., Barth, A., Chen, G.I., Tremper, A.H., Priestman, M., Ek, D., Gu, S., Kelly, F.J., Kalberer, M. and Green, D.C. 2024. 'High time resolution quantification of PM 2.5 oxidative potential at a Central London roadside supersite', *Environment international*, November 2024. [Online]. [Accessed: 22 January 2026]. Available from: https://leeds.primo.exlibrisgroup.com/discovery/fulldisplay?docid=cdi_pubmed_primary_39520930&context=PC&vid=44LEE_INST:VU1&lang=en&search_scope=My_Inst_CI_not_ebsco&adaptor=Primo%20Central&tab=AlmostEverything&query=any,contains,london%20air%20quality&facet=searchcreationdate,include,2023%7C,%7C2026&facet=topic,include,Environmental%20Sciences&offset=10

Ma, L., Graham, D.J. and Stettler, M.E.J. 2021. 'Has the ultra low emission zone in London improved air quality?', *Environmental research letters*, December 2021. [Online]. [Accessed: 22 January 2026]. Available from: https://leeds.primo.exlibrisgroup.com/discovery/fulldisplay?docid=cdi_iop_journals_10_1088_1748_9326_ac30c1&context=PC&vid=44LEE_INST:VU1&lang=en&search_scope=My_Inst_CI_not_ebsco&adaptor=Primo%20Central&tab=AlmostEverything&query=any,contains,london%20air%20quality&facet=searchcreationdate,include,2020%7C,%7C2026&offset=0

MacKerron, G. and Mourato, S. 2009. 'Life satisfaction and air quality in London', *Ecological economics*, March 2009. [Online]. [Accessed: 22 January 2026]. Available from: https://leeds.primo.exlibrisgroup.com/discovery/fulldisplay?docid=cdi_proquest_miscellaneous_58807021&context=PC&vid=44LEE_INST:VU1&lang=en&search_scope=My_Inst_CI_not_ebsco&adaptor=Primo%20Central&tab=AlmostEverything&query=any,contains,london%20air%20quality&offset=0

Tong, C., Dai, Y., Cole, M., Elliott, R.J.R., Bartington, S.E., Liu, B. and Shi, Z. 2025. 'Further improvement in London's air quality demands more than the Ultra Low Emission Zone policy', *NPJ Clean Air*, October 2025. [Online]. [Accessed: 22 January 2026]. Available from: https://leeds.primo.exlibrisgroup.com/discovery/fulldisplay?docid=cdi_proquest_miscellaneous_3265461113&context=PC&vid=44LEE_INST:VU1&lang=en&search_scope=My_Inst_CI_not_ebsco&adaptor=Primo%20Central&tab=AlmostEverything&query=any,contains,london%20air%20quality&offset=0
