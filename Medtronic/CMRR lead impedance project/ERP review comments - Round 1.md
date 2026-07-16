1. I note that berk has a personal Gmail listed. Does he have any university email? If so, please use the university email.
2. Update INS devices to Percept PC or RC
3. "labelling" to "labeling" in background
4. Expand on background to include a little more about the exact proposed method. Something like "There is a clear clinical and commercial need for a personalized, real-time measurement tool that can quantify and mitigate risk during the exam itself. By measuring the source of risk, aka tissue temperature, this personalized real-time risk evaluation would be possible."
5. "A Sensor Q-matrix (Qs) will be calculated in under 10 seconds using fast RF excitation delivered from the individual channels of the RF coil. The temperature-impedance relationship will be used to ensure the maximum temperature increase is limited to 0.7°C. A safe RF excitation scenario will be calculated using the Qs and verified with simultaneous impedance and temperature data measured during high-SAR clinical sequences. Finally, a clinical workflow will be developed to standardize this in situ, sensor-driven method toward a personalized implant safety approach, utilizing the existing hardware capabilities of DBS systems." 
   I like the Q matrix generation. It is a logical step to definitively show that standard B1+ or scanner reported SAR can have extreme disagreement with lead heating. On Medtronic's side, we are interested in a slightly more robust characterization than the proposed 0.7C increase. We strongly suggest the following updates
	1. An increase of the proposed temperature range. Something like increasing temperature change somewhere between 4 and 8C. This can be done by switching the sign in your x'*Q*x optimization ( min_x {-x'Qx} )
	2. Increase the number of implant locations. Instead of just measuring this in the brain, also see if it is possible for your vet team to implant in the  Epidural space of the spinal canal (for SCS pain management), sacral foramen for SNM, 
	3. Ensure the use of multiple heating and cooling curves to characterize temporal stability in the method.
	   
6. "In order to obtain data in a wide range with limited RF power, we will use a toroidal transceiver to deliver RF energy directly to the electrodes and to elevate the temperature. The relationship between the change in impedance/ temperature with respect to baselines will be fit to a mathematical model." 
	1. Could you use higher RF powers from the actual birdcage transmitter of the 3T system? Pointing back to comment 5.1, we are interested in higher temperatures as well that a toroidal transceiver might not be able to deliver.
	2. How feasible would a longitudinal study be where animals are implanted for ~3weeks before imaging/heating experiments are conducted? This data would be of high interest.
7. Primary Endpoints
	1. First endpoint should be "determine viable methods to retrieve INS impedance measurements during MRI scanning"
	2. " Validation of in situ impedance measurements as a reliable predictor of RF-induced heating at the implant electrodes during 3T MRI."
		1. Change to "Characterization of the variability in the correlation of impedance to tissue heating at the implant electrodes during 3T MRI". This is more in-line with the exploratory nature of the study. Validation seems to imply that this is known to work and also give a single value. We would be more interested in the accuracy of the model which is better captured by in the above recommendation.
	3. Change "A quantifiable reduction in RF-induced temperature rise (e.g., maintained below a specific threshold like 1°C) at the implant leads using subject-specific RF shimming." to
	   "A quantitative evaluation of the variability of tissue heating at a constant scanner reported B1+ or SAR"
	4. Add in another endpoint of "An analysis to quantitatively derive the required temporal resolution of the impedance measurements". This will answer the question that Burk did not have a great answer to of "what sampling rate do you need from Medtronic". The response was "faster the better", which is obvious, but we really are interested in a true lower bound and rational for this lower bound.

8.  "A wireless link via the sponsor's telemetry interface will transmit real-time impedance measurements to a console outside the MRI suite. 
	1. add in "This console could be either the clinician programmer tablet or a labprogrammer device."
9. "The subject will be exposed to specific MR imaging sequences using the scanner's standard 2-channel transmit body coil. The intervention compares two RF modes targeting identical scanner-reported B1+rms values: Standard Circularly Polarized (CP) mode (Control) and Our impedance-driven, Implant-Friendly (IF) 2-channel pTx mode (Test)"
	1. Add in a third "Implant-hazardous" mode
10. Secondary Endpoints
	1. Quantitative evaluation on the impact IF modes have on B1+ homogeneity and image quality for multiple high power sequences (3D TSE/SPACE, 2D TSE, T1 weighted TSE, FLAIR, etc.)
	2. remove "verification that measurement..." from this secondary endpoint as it should now be a primary endpoint
11. "There is a strong positive correlation between dynamic changes in electrode impedance and simultaneous RF-induced temperature rise at the electrode-tissue interface"
	1. Isn't it technically a positive correlation with electrode admittance?
12. "Therapies: It ensures patients do not have to choose between receiving your life-changing therapies (such as neuromodulation) and having access to future medical imaging." 
	1. Add in something along the lines of "Thereby reducing INS burden to patients"

In regards to requested products:
1. 6 x Percept PC devices ( 4 backups ) (B35200)
2. 6 x Sensight leads ( 4 backups ) (B3301533)
3. 3 x 95cm SS extensions ( 2 backups ) (B3400095)
4. 3 x 40cm SS extensions ( 2 backups ) B3400040)
5. 6 x legacy leads ( 4 backups ) (3389S-40) (this model is 0.5mm electrode spacing, Sensight is 1.5mm spacing, should be interesting to compare)
6. 3 x 95cm legacy extensions ( 2 backups ) (37085-95)
7. 3 x 40cm legacy extensions ( 2 backups ) (37085-40)
8. 3 x 8880T2 communicators (2 for the two INS devices implanted and 1 for backup) (8880T2)
9. 3 x Clinician programmers (2 for the two INS devices implanted and 1 for backup)
10. 2 x TMTI lab programmer communicators (No backups)

