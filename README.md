# Protesting Property’s Appraised Value 2023: Residential Property in Cedar Park, Texas

By: Sonali Agrawal

## Objective

The aim of this project is to protest the property taxes for our home in Cedar Park, Texas by gaining a thorough understanding of the district’s property value appraisal process. We will study the district's appraisal report, which includes the comparable properties used to calculate the appraised value of our property. These comparable properties are from the same neighborhood and share similar sizes. We will pay close attention to the appraisal process, particularly the calculations and adjustments made for improvements, such as decks, covered patios, garage. Following our understanding of the appraisal process, we will gather information, including details on improvements, for all properties within our neighborhood that are comparable in size to ours. We will make the necessary adjustments for improvements and calculate the appraised value of these properties. Our objective is to identify properties with lower appraised values than ours within the neighborhood. By presenting these comparable properties, we intend to build a strong case for a justifiable drop in the appraised value of our home, ultimately advocating for fair and accurate property taxation.

The Williamson Central Appraisal District (WCAD) assesses the value of properties within the county. They collect information about the property, including its size, location, features, and improvements. Once the WCAD determines the appraised value, they notify the property owner. This typically occurs around April or May of each year. The notice includes information about the appraised value, exemptions, and instructions for filing a protest if the property owner disagrees with the assessed value. If a property owner believes the appraised value is incorrect, they can file a protest with the Williamson County Appraisal Review Board (ARB). The ARB is an independent panel that reviews property tax protests. Property owners must provide evidence to support their claim. After considering the protests, the ARB makes a determination on the appraised value. The WCAD then updates the appraised value accordingly. The property tax is calculated based on the appraised value and the tax rate set by various taxing entities, such as the county, school district, and other local governments.

## Data Access

The Williamson County Appraisal District (WCAD) website serves as a valuable resource for accessing property information in the county. Through the website, users can easily search for specific properties and obtain relevant data. We downloaded the initial list of properties in the same neighborhood as the subject property. This list included information on property ID, address, appraised value for 2023 and WCAD link for more information. To enhance our analysis, we utilized the Selenium framework in Python to scrape the house size (in square feet) for all the properties in the downloaded list. We then applied a filter to the scraped dataset, focusing on properties within 100 square feet of our own property. The list included 123 properties. Further, we scraped information on improvements and appraised values for the filtered 123 properties.

## Analysis

When comparing the subject property (our house) to comparable properties, we took into consideration any improvements. Value adjustments were made to the appraised value based on these disparities. If a comparable property was deemed superior to the subject property in a particular attribute, a downward adjustment was applied to its appraised value. Conversely, if a comparable property was found to be inferior, an upward adjustment was made. By incorporating these adjustments, we obtained an indication of the ideal subject property's appraised value.

We considered adjustments for specific improvements, namely Garage, Open porch, Deck, Patio, and Fireplace. The subject property itself includes a Garage, Deck, Open porch, and Fireplace. However, there were other improvements (such as pool, outdoor kitchen) for which we lacked information regarding the adjustment value, and consequently, we excluded them from the calculation of the adjusted appraised value.

Following the calculations to determine the adjusted appraisal value for all properties within the neighborhood, we carefully selected 10 properties that were within 50 feet of the subject property's size and had the lowest appraised values. Additionally, we chose 10 properties within 100 feet of the subject property's size with the lowest appraised values. These selections are intended to be presented as compelling evidence during the protest hearing to support our case for a fair property tax assessment.

## Conclusion

During the protest hearing, we presented 2 lists of properties as evidence. The first list consisted of 10 properties within 100 feet of the subject property's size, while the second list comprised 10 properties within 50 feet of the subject property's size. Most of these properties had lower appraised values compared to the subject property. As a result, the mean appraised value of these properties was calculated to be lower than the value initially shared by the district.

This successful demonstration allowed us to effectively reduce the appraised value of our own house by $10,000. Our diligent analysis and the compelling evidence we provided played a crucial role in achieving this positive outcome during the protest hearing.

*Figure 1: Screenshot of the report with information on 10 comparable properties within 50 feet of the subject property's size*

![Comparable Properties](/Comparable_Properties.png)

## Data Dictionary

In the table below, we have provided a short description of the data variables which we have referred to in this project.

| Attribute  | Description  | Data Type  | Source  | Example  |
| --- | --- | --- | --- | --- |
| Property_ID  | A unique identifier per property  | Object  | WCAD  | R341326  |
| Address  | Address of the property  | Object  | WCAD  | 1607 PAPER MOON DR, CEDAR PARK, TX 78613  |
| Value_2023  | Appraised value  | Object  | WCAD  | 531745  |
| Link  | WCAD link  | Object  | WCAD  | https://search.wcad.org/Property-Detail/PropertyQuickRefID/R341326  |
| area  | Carpet area  | Object  | WCAD  | 2,714 Sq. Ft  |
| imp1  | Improvement details  | Object  | WCAD  | 1 Main Area 1997 1,357 N/A Details  |
| imp2  | Improvement details  | Object  | WCAD  | 2 Second Floor 1997 1,357 N/A Details  |
| imp3  | Improvement details  | Object  | WCAD  | 3 Garage 1997 399 N/A Details  |
| imp4  | Improvement details  | Object  | WCAD  | 4 Open Porch 1997 107 N/A Details  |
| imp5  | Improvement details  | Object  | WCAD  | 5 Open Porch 1997 462 N/A Details  |
| imp6  | Improvement details  | Object  | WCAD  | 6 Fireplace 1997 1 N/A  |
| imp7  | Improvement details  | Object  | WCAD  | 7 Out Bldg 1999 120 N/A Details  |
| imp8  | Improvement details  | Object  | WCAD  | 8 Concrete Pool 2003 399 N/A Details  |
| imp9  | Improvement details  | Object  | WCAD  | 9 Fireplace 1994 1 N/A Details  |
| imp10  | Improvement details  | Object  | WCAD  | 10 Open Porch 2021 268 N/A  |
