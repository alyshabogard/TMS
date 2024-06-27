# TMS (in MATLAB)

Able-bodied subjects participated in a pre-post study design to assess changes in corticospinal excitability to the tibialis anterior muscle after five consecutive days of AIH. We generated recruitment curves by plotting the peak-to-peak MEP amplitudes against the normalized stimulus intensities based on the participant’s resting motor threshold. To assess changes in corticospinal excitability, we quantified TMS indices such as changes in the maximum MEP amplitude (MEPmax), the area under the recruitment curve (AUC), the peak slope of the recruitment curve, and resting motor threshold (RMT). 

The MEP onset was identified using custom configurations in Signal software (CED, USA) as the first frame at which the peak-to-peak amplitude exceeded 3 SD of the background EMG. Background EMG was the peak-to-peak average recorded 200 ms preceding the TMS stimuli. Mean background EMG was subtracted from all MEPs. RMT represents the motor threshold required to excite the TA at rest in 4/7 trials.

AUC was calculated using the trapezoidal method of area estimation. The recruitment curve slope was determined by fitting a Boltzmann distribution in MATLAB using the Levenberg-Marquardt algorithm. Briefly, the Boltzmann equation is a function of stimulus intensity (s) and response amplitude (MEP), where  MEPmax is the maximum averaged response from the recruitment curve, s50 is the stimulus intensity required to produce a response with half the amplitude of MEPmax, and k is the slope parameter. Peak slope, the inverse of the slope parameter, represents the rate of the MEP increase relative to MEPmax.

MEP(s) = MEPmax/(1+e^(((s50-s))⁄k))
