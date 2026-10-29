# IITR-CAPSTONE-PROJECT
I have joined a company named DELHIVERY which has the largest logistics network in India.
I have joined as an analyst to a regional team.
there a promised deadline for delivering a parcel that is express(36hours), standard(60hours) and economy(96hours).
the delivery head has three main problems to tackle without having a pipeline(workflow).
Problems are: 1.how long will a parcel take? 2. which parcels are delayed from their actual promise time to be delivered? and 3. nobody actually knows how the 24 different hubs are actually working and fulfilling customers demand.
there are 4 parts to the problem which connected to each other that is if any part or step is having issues will cause others to fail significantly.
part A(cleaning and feature codes), part B(regression), part C(classification) and part D(hub segments are linked with final scoring script). all the parts are interrelated in a continuous way that each part depends on the previous part.
PART A: Provided data — generate_data.py   Part A — Data Foundation and Delay Evidence
Repository and data. Create the repository, commit generate_data.py requirements are:
clean_shipments(raw, medians=None) in src/shipment_prep.py,   
drop duplicate rows
striping and converting to title, service_type
replace a placeholder "Unknown" for missing value in column payment_mode,
removing rupee sign and commas from column declared_value and change it to new name as declared_value_inr
convert column dispatch_time to a datetime
If the value in column parcel_weight_kg exceeds 100 treat it as missing
fill the columns distance_km, parcel_weight_kg and declared_value_inr with their column's median
build_features(clean, hubs) in src/shipment_prep.py.
part_a_clean_eda.py.
Checks file
elay evidence table.
Correlations. Write outputs/part_a_correlations.csv
write at least four findings, each quoting a number copied from your own output files
