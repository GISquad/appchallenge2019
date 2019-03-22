# Sustainera by GISquad
Sustainera is a web application that estimates the potential energy and CO2 savings of buildings and neighborhoods in Toronto, Ontario

### Team
* Matthew Brown: Lead Designer
* Tasos Dardas: Lead Developer
* Michele Tsang: Lead Researcher 

## Mission Statement

In Canada, buildings account for almost a third of its’ annual greenhouse gas (GHG) emissions. As Canadian cities continue to grow, so does the demand for energy. Buildings have a substantial impact on the environment as they use resources, generate waste and are costly to maintain and operate. There is high potential to deliver significant cuts in emissions at very little costs, benefiting the environment, economy and society. With new constructions, renovations or retrofits, buildings in Toronto can achieve superior levels of energy efficiency by using fewer resources, reducing waste, improving air quality and eliminating negative environmental impacts. 

Toronto’s population is projected to grow over 35% by 2050, which will further the expansion of residential and commercial infrastructure. In 2010, the City of Toronto implemented the [Toronto Green Standard](https://www.toronto.ca/city-government/planning-development/official-plan-guidelines/toronto-green-standard/toronto-green-standard-overview/), which are sustainable design requirements for new private and city-owned developments. This includes a performance target for new buildings to approach zero emissions by 2030. [Toronto’s Climate Action Strategy](https://www.toronto.ca/wp-content/uploads/2017/11/91f6-TransformTO-Modelling-Torontos-Low-Carbon-Future-Results-of-Modelling-Gr....pdf) also has a city-wide goal of achieving an 80% reduction in GHG emissions by 2050. These targets not only reduce carbon emissions but also make Toronto’s buildings more resilient, comfortable and affordable with lower energy costs.
 
Our app, Sustainera, aims to promote sustainable buildings using 2 strategies; reducing energy/water consumption and planting green rooftops. Choosing efficient insulation, lighting and appliances saves energy, lowers utility bills, increases indoor comfort and reduce impacts on the environment. Green roofs act as a rainwater buffer, reduce noise and air pollution, regulate indoor temperatures by providing extra insulation and absorb CO2, making urban areas less likely to become heat islands. Buildings that choose to be more sustainable will face higher initial costs, but the difference will be easily recovered over time through energy savings. Not only do green buildings benefit tenants and households with savings in utilities, but they also lower maintenance costs and increase property value for building developers.  
  
      
## App Description & Features

**1. Neighborhood Statistics**  
By selecting a neighborhood, the user can identify the number of existing buildings and the proportion that is residential and non-residential. Based on the total area of these buildings, the number of LED light bulbs required for upgrading from incandescent can be estimated, which is used to calculate the savings in dollars over the lifespan of the light bulbs. This informs the user of the net savings of neighborhoods as the value accounts for the cost of LED bulbs. Switching to LED not only has monetary savings but also reduces CO2 emissions by using less energy. The equivalent savings in pounds of CO2 is also estimated from upgrading to LED bulbs for a neighborhood. The total area of buildings within a neighborhood is also used to calculate the number of possible rooftop trees that can be planted. Based on the number of trees, the amount of CO2 emissions, in pounds, that can be absorbed by them can also be estimated. 

**2. Building Statistics**  
After the user selects a neighborhood, buildings can be symbolized in 3D by 6 different categories, the height of a building, type of building (residential versus non-residential), LED savings (dollars), number of rooftop trees, the amount of CO2 reduced from LED light bulbs or the amount of CO2 reduced from rooftop trees. Similar to the neighborhood statistics, the LED savings (dollars) can be determined based on the area of a single building, as well as the amount of CO2 reduced (pounds) from LEDs using less energy. The area of each building also estimates the possible number of rooftop trees that can be planted, which is also used to determine the amount of CO2 that can be potentially absorbed.


**3. Return of Investment (ROI) Calculator**   
The ROI Calculator provides the user with an estimate of the number of years it takes for their money to be made back from switching to spray foam insulation, 4.8L/flush toilets, high efficient washing machines and/or gas dryers. Using inputs from the user, such as the area they want to insulate, the number of toilets they want to upgrade or the number of people in the household, dynamic ROI times can be estimated. The value returned is based on the cost of upgrades and installation and the savings in utilities. After the ROI period, the user will only be saving money from switching over to these highly efficient options.   
   
  
## User Manual
  
To launch the app, click here
1. Select a neighborhood in Toronto or use the search function and type in an address to navigate to its neighborhood.  
2. The default view of the app is in 3D, but can easily be switched to 2D by selecting the 2D button at the top.  
3. Click on a building and a pop-up will appear that gives 6 statistics about its’ height, type, LED savings in dollars, LED savings in CO2 reduced, number of rooftop trees and CO2 reduced from rooftop trees.  
4. In the top-left of the app, click on the 3 horizontal lines icon and select the “Info” button to bring up a menu that allows you to visualize different statistics, view your neighbourhood summary, and calculate ROI.   
5. From the dropdown under “Select Information”, click “Building Stats” to view the same 6 statistics as shown in the popup. Here, values from any of these 6 statistics can be used to symbolize the colour and height of the buildings.  
6. Under “Select Information”, switch from “Building Stats” to “Neighborhood Stats” to see an overview of the selected neighborhood’s efficiency potential.  
7. Under Select Information, switch from “Neighborhood Stats” to “Calculate my ROI” to estimate your ROI for any of the 4 sustainable options. For Insulation, input the square footage of your household and the cost of your monthly energy bill. Under Water, input the number of toilets you want to upgrade in your household/building and the number of people occupying that space. To determine the ROI for an efficient washer and/or gas dryer, input the number of people in your household.   

## Calculations and Assumptions 

**Lighting**

|          |      LED      |  Incandescent |
|----------|-------------:|------:|
| Lifespan (hours) |    25000 | 1200 |
| Watts per bulb |   8.5 | $12 |
| Cost per bulb |   $4.00 | $2.00 |
| KWh of electricity used over 25 000 hours |   212.5 | 1499.76 |
| Cost of electricity (@ $0.094 per KWh) |   $19.98 | $140.98 |
| Bulbs needed for 25 000 hours of use |   1 | 21 |
| Equivalent 25 000 hours bulb expense |   $4.00 | $42 |
| Total Cost for 25 000 hours |   $23.98 | $182.64 | 
|                                                      |                 
| Energy Savings over 25000 hours assuming 25 bulbs per household | 
| Total Cost for 25 bulbs | $599.38 | $4,566.10|
| Savings to household from switching to incandescent | $3,966.73||


The savings from replacing incandescent light bulbs with LED light bulbs are based from the values above. It also assumes 5000 lumens are required for every 250 square feet and each bulb produces 800 lumens (LED and incandescent). The cost of lightbulbs are based on the average prices found in Toronto. The cost of electricity is based on mid-peak prices for Ontario. To convert the area from square meters to square feet, the area of the building is multiplied by 10.7639. The total monetary savings is based on the lifespan of LED light bulbs.   

*Savings ($) = (((((Area of Building in m2x10.7639)/250)x5000)/800)/25)x3966.73*  

The equivalent savings in CO2 is based on the fact that 7.07 × 10-4 metric tons CO2 is saved per kWh. 1287.26 is the amount of kWh savings from switching a single bulb from incandescent to LED.  

*Savings (metric tons of CO2) = ((((((Area of Building in m210.7639)/250)*5000)/800)/25)*1287.26)*0.000707*  

Both the monetary and CO2 savings from switching to LED light bulbs is based on the area of building footprints, so it does not account for multiple floors. To obtain savings for multi-floor buildings, the user can multiply their savings by the number of floors.   
 
**Insulation**  

In Toronto, spray foam insulation ranges from $1.75 to $3.00 per square foot with an average professional installation cost of $2021. The calculation used assumes a cost of $2.00 per square foot and a spay depth of 1 inch. Based on previous case studies, spray foam insulation reduced a household’s monthly energy bill by an average of 48%. Therefore, in this calculation, we will assume installing spray foam insulation will reduce the monthly energy bill of the user by 40%. The monthly energy savings is multiplied by 12 to obtain ROI in years.   

*ROI (years) = (building square foot*2+2021)/((Cost of Monthly Energy Bill*0.4)*12)*

