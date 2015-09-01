# 2015-LCD-PhillyViolations
All violations from the Licences and Inspections database in one place. The data was scraped on August 1, 2015 from the Licenses and Inspections Violations API found here: http://phlapi.com/licenseapi.html.

In total, 1,077,623 violations were successfully extracted from the Licenses and Inspections database. Each violation is linked to a L&I case, as well as to a location. The extracted violations could be grouped into 368,574 unique cases, or 157,350 unique locations.

The data is formatted in 12 comma-separated value (CSV) files. Each CSV file contains approximately 89,800 records, small enough to be opened in most spreadsheet editors.

Each record has 27 descriptive data fields. Data fields may not be available for each database record: in that case, the field for that record is listed as "None." The fields are as follows:

1. ViolationID (Integer, ID): A unique ID that can be used to search each violation in the License and Inspection database
2. ViolationCode (Text): The specific section of the housing code that has been violated
3. ViolationCodeDescription (Text): A short visual description of the violation
4. ViolationDate (Date): The date when the violation was recorded. Dates from the L&I database are formatted in the format '/date(###########)/', where the numbers within the parentheses represent milliseconds since 1970 
5. ComplianceStatus (Text): Classifies the property owner's compliance in fixing the violation: either “Complied” or “Not Complied”
6. ViolationLocation (Text): Verbal description of the violation's location on the property
7. CaseNumber (Integer, ID): The case ID for this violation, which can be used to search for the case in the License and Inspection database
8. LocationID (Integer, ID): A unique ID that can be used to search for the violation location in the License and Inspection database
9. CaseType (Text): Describes the city program that is pursuing this case
10. CaseLocation (Text): Partial description of the case location, if all violations within a single case were identified within a single area of the property
11. AddedDate (Date): The date when the violation was added to the database. Dates from the L&I database are formatted in the format '/date(###########)/', where the numbers within the parentheses represent milliseconds since 1970 
12. LastUpdatedDate (Date): The date when the violation record was last updated in the database. Dates from the L&I database are formatted in the format '/date(###########)/', where the numbers within the parentheses represent milliseconds since 1970
13. Resolution (Text): Describes whether the case was closed by the property owner (“Closed”), resolved by city action (including “Sent to Court” and “Clean and Seal”), or is currently still open (“Open”)
14. ResolutionDate (Date): The date when the case was resolved.  This field is left blank for currently-open cases. Dates from the L&I database are formatted in the format '/date(###########)/', where the numbers within the parentheses represent milliseconds since 1970
15. Priority (Text): A classification of the violation's threat to human health. Ranges from “Non-Hazardous” to “Imminently Dangerous”
16. StNum (Integer): The street number of the violation location
17. StDir (Letter): The directional prefix (N, E, S, W) of the street, if one exists
18. StName (Text): The name of the street
19. StSuffix (Text): The type of street (ST, AVE, DR)
20. ZIP (Text): The nine digit ZIP code for the violation location, in "#####-####" format
21. x (Integer): This can be used to locate the violation in space using the State-Plane Coordinate Reference System (in feet)
22. y (Integer): This can be used to locate the violation in space using the State-Plane Coordinate Reference System (in feet)
23. CensusTract (Integer): The census tract in which the violation occurred
24. CouncilDistrict (Integer): The council district in which the violation occurred
25. CondoUnit (Integer): For condominiums, the specific condo unit in which the violation occurred
26. UnitNumber (Integer): For apartments, the specific apartment in which the violation occurred
27. Ward (Integer): The city ward in which the violation occurred

~~~~~~~~~~~~~~~~~~

This repo is a result of data analysis completed as part of the Summer of Maps Program. This work was completed in support of a pro bono project with the Legal Clinic for the Disabled.

Summer of Maps is a fellowship program organized and facilitated by Azavea. Azavea is a B Corporation that specializes in civic-minded GIS software development and spatial analysis. Summer of Maps offers stipends to student spatial analysts to perform data analysis and visualization for non-profit organizations. Every year we match up non-profit organizations that have spatial analysis needs with talented students to implement projects over a three-month period during the summer.

The 2015 Summer of Maps program is sponsored by Esri, Temple University Professional Science Masters in GIS and Betsy and Jesse Fink.

