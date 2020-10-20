# data_high-z_mock
The mock catalogs of zCOSMOS survey and PFS survey, the catalog for zCOSMOS-bright sample and the measurement of LF, GSMF, projected 2PCF with zCOSMOS-bright sample. Paper: <https://arxiv.org/abs/2008.13733>
## Mock catalog
We have constructed the mock catalogs for zCOSMOS survey and PFS survey. 
The mock catalogs can be downloaded from <https://lig.astro.tsinghua.edu.cn/astrodata/>. Or you can contact <mengjc18@mails.tsinghua.edu.cn>.
## The catalog for zCOSMOS-bright sample
The file data/zcosmos_sample.fits stores this catalog.
It is secure to use the galaxies with Flag = 1 and in the central region.

That is (Flag == 1) & (Center_region == 1)

>1. ID
2. RA : J2000
3. Dec : J2000
4. ID_2015 : ID in COSMOS2015 catalog
5. z_spec : spectroscopic redshift
6. Type : 0 for galaxies; 1 for stars; 2 for X-ray sources
7. Mass : stellar mass, unit: $M_{\odot}$.
8. Flag : 1 for well matched galaxies with secure redshift
9. CC : confidence class of spectroscopic redshift (Lilly et al. 2009).
10. Weight : weight for each galaxy
11. Center_region : 1 for galaxies in the central region of zcosmos survey 149.62<RA<150.61 and 1.75<DEC<2.70
12. m_I : apparent magnitude of I band (HST 814W)
13. M_I : absolute magnitude of I band (HST 814W)
14. M_B : absolute magnitude of B band

The file data/zcosmos_random.fits stores the random sample. The redshift range is 0.1~1.5. It only contains the points in the central region.

>1. RA : J2000
2. Dec : J2000
3. z : redshift
4. Mass : stellar mass, unit: $\log(M_{*}/M_{\odot})$
5. m_I : apparent magnitude of I band (HST 814W)
6. M_I : absolute magnitude of I band (HST 814W)

## COSMOS2015 catalog
<ftp://ftp.iap.fr:/pub/from_users/hjmcc/COSMOS2015>

## Measurements of zCOSMOS bright sample
The measurements of LF, SMF and projected 2PCF are in the data/zCOSMOS_bright_measure
