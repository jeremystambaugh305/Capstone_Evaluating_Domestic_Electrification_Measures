# Project XYZ

**Project XYZ** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* Describe your dataset. Choose a dataset of reasonable size to avoid exceeding the repository's maximum size of 100Gb.


## Business Requirements
* This project will evaluate the current cost and carbon reduction potential for the following 3 major electrification measures available to households where none of these currently exists:

1. An electric car (Ecar)
2. A rooftop mounted solar PV array (Solar PV)
3. An air source heat pump (ASHP)

These are in my anticipated descending order of potential cost saving for an average home with gas heating and a petrol car.

## Hypothesis and how to validate?
* I anticipate the following results but these will be evaluated in this project:-

1. Out of the 3 options, Ecars, in particular secondhand, will have the greatest cost saving potential where home charging is available but this will be greatly diminished, possibly negated, where home charging is unavailable with all charging from public chargers.

2. Moderate long term potential cost savings from solar PV in households with high daytime occupancy, particularly if high energy electrical appliances are operated at times of high sun. But savings will be greatly diminished if daytime occupancy is low as current export values are low.  Incorporating battery storage may improve but only slightly as they have high up front costs.

3. No cost saving from air source heat pumps compared with gas heating as 
i) The up front costs of ASHPs are substantially higher than gas boilers even with the current government boiler upgrade grant support scheme (BUS) 
ii) The current ratio between electricity and gas prices is generally higher than the ratio between heat pump and gas boiler efficiency meaning air source heat pumps have higher fuel costs than gas boilers. 
The above cost disadvanteges are offset to a degree by ASHPs having longer anticipated life spans and lower maintenance costs, but these advantages seem unlikely to reverse the situation.

iii) All options will clearly reduce CO2 emissions but solar PV will have the lowest CO2 reductions in most cases due to the carbon intensity and generated electrical energy being much lower than the carbon intensity and displaced heating gas or car petrol consumption energy.  

iv) For an averahe household, Ecars and ASHPs displace a very similar amount of CO2, just over 2 Tonnes.  This is based on average annual car mileage of 7,100 miles at 45MPG and gas heating consumption of 11,500kWh at an efficiency of 86%GCV. So Ecars will likely displace more CO2 than ASHPs in households with a higher ratio of car mileage/heating consumption and vice versa.

These anticipated results will be evaluated by cost and carbon calculations using techno-economic data obtained from Kaggle, UK government and other public websites which will be analysed statistically and feature engineered as necessary before feeding these calculations.

Key data and outputs will be displayed in interactive dashboards using Power BI to visually demonstrate the up front costs and the cost and carbon saving potentials of each of these 3 measures, firstly under the likely range of domestic circumstances and secondly in more detail, those particular to each household.  The aim is to help households decide whether to proceed with one or more of these electriciation technologies and if so which one(s).  

This will be a general tool covering a broad range of situations using datasets some of which are changing quickly so soon outdated, so it is advised that this be followed up with more detailed and focussed analyses using the latest data.

## Project Plan

# 
### ECars

A techno-economic data (including up front costs, battery size, efficiency) were obtained from Kaggle.  Note this data was produced in 2023 so may be somewhat outdated.  For example some web searches indicate some cars no longer available, new cars available and some substantial price reductions so this data is likely to be conservative.  I have kept to this dataset as I know of no more recent comprehensive set but this would be a potential future improvement.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations
* Were there any data privacy, bias or fairness issues with the data?
* How did you overcome any legal or societal issues?

## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.

* Ecars. 
1. Key dashboard result - a bubble plot showing lifetime cost savings of the most economical Ecar for each mileage range and annual mileage combination (lowest up front or 8 year cost depending on user selection) by bubble size and colour on a 2 dimensional plot with range and annual mileage on the x and y axes respectively. This allows users to quickly and flexibly see a map of all scenarios, which are most favourable, if well known, the point on the map the range and annual mileage sits, or if uncertain the region of applicable scenarios to judge how much the best Ecar is likely to save them over 8 years for a new car or 4 years for a 4-year old used car.

Selectable variable setting variations on the above:-

i) Access to a home charger Y/N.
ii) Is the Ecar is new or second hand.
iii) Select cheapest based on up front or 8 year total cost.
iv) Counterfactual petrol car is an assumed equivalent or cheapest.
v) Whether assumed maintenance cost saving is low/med or high.

# Check, will I have to calculate all above scenarios in the Jupyter notebook i.e. multiplying table size by 2*2*2*2*3=48 then filter on the above in Power BI?  May just opt for Med maint cost saving to reduce data and simplify for user?

2. More detailed interactive plots filtered depending on range and annual mileage selection on main plot:-

i) Bar chart showing 

* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.


## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.