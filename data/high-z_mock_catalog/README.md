# high-z_mock_catalog
The mock catalog for high-z galaxy redshift survey. The details can be found in <https://arxiv.org/abs/2008.13733>. If you have any problems, please contact <mengjc18@mails.tsinghua.edu.cn>.

## PFS
The files in the folder PFS are the mocks for the PFS galaxy evolution survey main galaxy sample. The redshift range is 0.7~1.7. The selection criteria is 
>y < 22.5 for z < 1  
>y < 22.5 or J < 22.8 for z > 1

There are three field for PFS survey, E-COSMOS (ecosmos), XMM-LSS (xmmlss) and DEEP2-3 (deep). The file name is fiber_field_i.fits, where the "field" is the name of the field and the "i" indicates the i-th mock. We totally generate 20 mock catalogs.  

The columns in the file are  
1. ID: the id of the galaxy.  
2. gID: the id of the group the galaxy is in.  
3. ra.  
4. dec.  
5. z: redshift.  
6. stellar_mass: the mass of the galaxy, the unit is log10(M_*/M_sun).  
7. m_y: y-band apparent magnitude.  
8. m_J: J-band apparent magnitude.  
9. M_y: y-band absolute magnitude.  
10. M_J: J-band absolute magnitude.  
11. snap: the snap-shot of the galaxy in the simulation.  
12. halo_mass: the mass of the halo the galaxy in, the unit is 10^10M_sun/h.  
13. source_tag: 1 for central galaxies and 0 for satellites.  
14. pfs_tag: 1 for galaxies satisfying the selection criteria and 0 for not.  
15. fiber: 1 for galaxies are observed with known redshift and 0 for not.  

## zCOSMOS
The files in the folder zCOSMOS are the mocks for the zCOSMOS bright sample. The selection criteria is 
> I < 22.5  

The file name is zc_i.fits, where the "i" indicates the i-th mock. We totally generate 20 mock catalogs.  

The columns in the file are  
1. ID: the id of the galaxy.  
2. gID: the id of the group the galaxy is in.  
3. ra.  
4. dec.  
5. z: redshift.  
6. stellar_mass: the mass of the galaxy, the unit is log10(M_*/M_sun).  
7. m_B: B-band apparent magnitude.  
8. m_I: I-band apparent magnitude.  
9. M_B: B-band absolute magnitude.  
10. M_I: I-band absolute magnitude.  
11. snap: the snap-shot of the galaxy in the simulation.  
12. halo_mass: the mass of the halo the galaxy in, the unit is 10^10M_sun/h.  
13. source_tag: 1 for central galaxies and 0 for satellites.  
14. survey_tag: 1 for galaxies satisfying the selection criteria and 0 for not.  
15. TSR: 1 for galaxies are observed and 0 for not.  
16. SSR: 1 for galaxies with successful redshift measurement and 0 for not.  