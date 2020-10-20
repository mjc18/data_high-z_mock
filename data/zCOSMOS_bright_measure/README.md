# The galaxy abundance and clustering measured from zCOSMOS bright sample

We measure the B-band luminosity function, stellar mass function and projected 2PCF with the zCOSMOS bright sample. The details can be found in <https://arxiv.org/abs/2008.13733>. Here are our results.

## "luminosity_function_B.hdf5" 
B-band luminosity function measured from the zCOSMOS bright sample.
In the hdf5 file, 
> the group "LF_z1_z2" store the LF in the redshift range [z1, z2]
>> the members in the group are:  
>>"M_B": absolute magnitude of B-band  
>>"LF": value of luminosity function  
>>"LF_err": error of luminosity function  

## "stellar_mass_function.hdf5" 
Stellar mass function measured from the zCOSMOS bright sample.
In the hdf5 file, 
>the group "GSMF_z1_z2" store the GSMF in the redshift range [z1, z2]
>>the members in the group are:  
>>"Stellar_Mass": log10(M_*/M_sun)  
>>"GSMF": value of stellar mass function  
>>"GSMF_err": error of stellar mass function  

## "projected_2pcf.hdf5" 
Projected 2PCF measured from the zCOSMOS bright sample
In the hdf5 file,
>the group "wp_z1_z2" store the projected 2PCF in the redshift range [z1, z2]. The subgroups "mass_m1_m2" store the wp in the stellar mass bins [m1, m2], where the unit of m1 and m2 is log10(M_*/M_sun)
>>the members in the subgroup are  
>>"r_p": projected distance, unit is Mpc/h  
>>"wp": value of projected 2PCF  
>>"wp_err": error of projected 2PCF  

## "F_theta.hdf5"
The function f(\theta)=(1+w_p)/(1+w_s) to correct the fiber collision effect.
>the group "F_theta_z1_z2" store the f(\theta) in the redshift range [z1, z2]. The subgroups "mass_m1_m2" store the f(\theta) in the stellar mass bins [m1, m2], where the unit of m1 and m2 is log10(M_*/M_sun)
>>the members in the subgroup are  
>>"theta": angular distance, unit is degree  
>>"F_theta": value of f(\theta)
