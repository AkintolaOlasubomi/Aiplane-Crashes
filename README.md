# Aiplane-Crashes
**Analysis of Plane Crashes (1908 – 2009)** <br>
This is a capstone project for the <a href="https://techcommunity.microsoft.com/t5/educator-developer-blog/learning-data-analysis-curriculum-and-resources/ba-p/3497797">#30daysoflearning (Data Analyst track)</a> program by <a href="https://github.com/theoyinbooke">Olanrewaju Oyinbooke</a>. 
The dataset contains information on all plane crashes from 1908 till 2009. It has 5268 records with 12 attributes which include:
- **Date**: Date of accident, in the format - January 01, 2001
- **Time**: Local time, in 24 hr. format unless otherwise specified
- **Operator**: Airline or operator of the aircraft
- **Flight #**: Flight number assigned by the aircraft operator
- **Route**: Complete or partial route flown prior to the accident
- **AC Type**: Aircraft type
- **Reg**: ICAO registration of the aircraft
- **cn / ln**: Construction or serial number / Line or fuselage number
- **Aboard**: Total aboard (passengers / crew)
- **Fatalities** : Total fatalities aboard (passengers / crew)
- **Ground**: Total killed on the ground
- **Summary**: Brief description of the accident and cause if known

## Data Wrangling
### Quality Issues
- Blank Cells: Filled in all blanks with “Unknown”
- The location columns contained Cities, States, Countries, Islands. I only needed the countries, so I got it extracted using split to column and checked for their validity using python in Jupyter notebook.
- The Summary did not give a precise information as to what caused the aircrashes. I had to extract causes using keywords and categorize them into clusters.
  - The causes were categorized into Nine namely;
    - Overshot Runway: To fly or taxi beyond the runway during takeoff or landing.
    - Weather Condition: Crashes caused by terrible weather such as snowstorms and rainstorms.
    - Mechanical Failure: Malfunction of an airplane component
    - Pilot Error: Crashes caused by errors on the pilot’s side
    - Shot down: Plane crashes caused by shooting down the plane
    - Bomb: Explosion on plane
    - Struck an object: Crashes because of airplane hitting an object while in motion.
    - Fuel Exhaustion: Low fuel leading to crashes
    - Collision: Colliding with other planes 
    - Unknown Causes
   
   <a href=https://github.com/AkintolaOlasubomi/Aiplane-Crashes/blob/main/Airplane_Crash.pdf>View the report summary here.</a>
    
