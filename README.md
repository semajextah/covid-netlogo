# covid-netlogo
Netlogo simulation comparing mask efficacy over 90 minute flight on a boeing airplane 747-400.
This simulation depicts the 3 different masks types as depicted in various literature sources.
I obviously won't post my entire paper here but here is an exert that will provide information about masking.

**The first major factor is the mask efficacy**
The simulation will test 3 different masks and a scenario where the infected wearing no mask. 
The three different types of masks will be a homemade mask made from random cloth which has a median of 70% water droplet blocking efficiency, a single layer mask made from new T-shirt cloth that has a 81.9% median efficiency, a medical mask with 98.5% efficiency (Aydin et al.). 
Coughing without a mask has the possibility to travel up to 3 meters whilst coughing with a mask has an upper end of 1.5-meters of distance (Simha and Rao)

**The second major factor is setting up seat pitch & width to accurately simulate a coughing radius pattern, its important to note the coughing radius is elliptical due to the seat pitch / width ratio**
The seat width on a Northwestern owned Boeing 747-400 is 17.2 inches, or .436th of a meter. 
The seat pitch is 32 inches, or .8128th of a meter. 
We took both of those numbers and divided them into the 3-meter coughing distance and the 1.8-meter coughing distance. 
This gave us the number of chairs the cough could travel over inside of our modeled area. 
The cough could travel laterally 6.8 chairs without a mask and 3.4 chairs with a mask; 
if the infected is coughing forward the reach without a mask is 3.69 chairs and 1.8 with a mask.
If a cough overlapped 50% or more onto the next seat it was included as a potentially infected person.
The elliptical radius serves 2 purposes, it increases the accuracy of our model due to the 1:1 scaling of our model and because we could not accurately predict which way the ‘infected’ would turn his or her head, therefore everyone within the maximum coughing distance is considered in range. 
Combining these two aspects we have the coughing variable randomly assigned a mitigation factor, depending on the type of mask they are wearing, it will either prevent the droplet from exiting the mask or go to its maximum coughing distance. 
The respective mitigation factors will correspond with the layer’s protentional blocking value from 0%, 70%, 81.9%, and 98.5%.


References
Aydin, Onur, et al. “Performance of Fabrics for Home-Made Masks against the Spread of COVID-19 through Droplets: A Quantitative Mechanistic Study.” Extreme Mechanics Letters, Elsevier, 11 Aug. 2020, www.sciencedirect.com/science/article/pii/S2352431620301802. 


Simha, Padmanabha Prasanna, and Prasanna Simha Mohan Rao. “Universal Trends in Human Cough Airflows at Large Distances.” AIP Publishing, AIP Publishing LLC AIP Publishing, 1 Aug. 2020, aip.scitation.org/doi/full/10.1063/5.0021666. 


My results
Groups	Count	Sum	Average	Variance
No mask	1000	21047	21.047	41.57836937
Homemade Mask	1000	7410	7.41	4.05995996
Single Layer	1000	5608	5.608	2.927263263
Medical Mask	1000	705	0.705	0.658633634
