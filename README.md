Download link :https://programming.engineering/product/mae-119-homework-3/

# MAE-119-Homework-3
MAE 119: Homework 3
You must show all work for full credit. Joint submissions can be made in groups of two. All submissions and code must be uploaded to Canvas for full credit.

Problem 1 (100 points)

We will study the real PV generation of the PV array located at the Gilman Parking structure.

(15 points) Convert GHI to POA: Load the measured GHI data into Matlab (\measuredGHI2016.mat”). Transform GHI to DIF and DNI using the Erbs decomposition model (\pvl erbs”). Calculate the POA for the panels at the Gilman parking structure by correcting the di use using the Perez model (\pvl perez”) and considering that the panels are tilted 10 facing south in a site with albedo 0.2. Find the days with the largest and smallest total daily POA and plot GHI and POA for those days.

(15 points) Convert POA to DC power: We will use the Sandia Array Performance Model, which needs the PV module and array data, and meteorological conditions to obtain the operational cell temperature. In order to do this, rst nd and load the data for the PV module at Gilman: \Kyocera KD 205 GX-LP”. The system at Gilman is composed of 2 arrays and 952 PV modules, so we can model just 1 array with 17 strings of 28 panels connected in series, and afterwards we will need to duplicate the generation. Use the measured meteorological data (\measuredMeteorological2016.mat”). What is the total DC energy generated over the year? What is the maximum cell temperature?

(15 points) Convert DC power to AC power: Load the data for the inverter \Xantrex GT 100″, and convert DC power to AC power (\pvlib snlinverter”). There are 2 of these inverters at the Gilman Parking structure, so we need to duplicate the AC generation in order to obtain the actual output power to the grid. Find the days with the largest and smallest total daily DC power and plot the DC and AC power for those days. Plot inverter e ciency versus inverter power factor, which is de ned as DC power over inverter power rating.

(20 points) Compare inverter size: Repeat the calculations for 1 array varying the inverter sizes between 10 and 500 kWAC. (To do so, modify the ‘Inverter’ parameters ‘Pac0’, ‘Pdc0’, ‘Ps0’, and ‘Pnt’ proportionally.) Plot the total annual AC power generation in MWh/a versus the inverter capacity (AC power), and also the total annual AC power generation versus inverter price pinv given by

pinv ($=kWAC) =

(

97:5 0:075 PAC

AC

100 kW

PAC

500 kW

145:556 0:556 P

10 kW

PAC

100 kW

where PAC is the inverter size in kW. Which inverter would you buy?

(15 points) Temperature e ects: Vary the yearly ambient temperature by (-4,-2,2,4) C. Plot the total annual AC power generation in MWh/a versus the temperature change, and determine the panel temperature coe cient at the maximum power point.

(20 points) Evaluate real and modeled generation: Load the real AC generation from the Gilman Parking structure into Matlab (\realACPower2016.mat”). For the real and modeled generation (computed in parts 2 and 3), compute all the performance metrics that are applicable to each dataset: array yield, nal yield, reference yield, panel e ciency, inverter e ciency, system e ciency, performance ratio, and capacity factor. Discuss the di erences between modeled and real data.

