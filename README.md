
BOSS DR12 data & mocks splitted in 6 bins, the samples used in arXiv:1609.05476.

3 bins in LOWZ, 3 bins in CMASS:

	In Redshifts, the BOSS simulation is split according to: 
	 z = [0.15, 0.2741, 0.35103, 0.43, 0.51131, 0.57195, 0.6929] 

	In Omega=0.26 LCDM, the BOSS simulation is split according to: 
	 r = [436.07, 775.25, 975.38, 1172.74, 1367.47, 1507.22, 1772.34] Mpc/h

	In Omega=0.3071 LCDM, the BOSS simulation is split according to: 
	 r = [433.774, 767.908, 963.711, 1155.839, 1344.491, 1479.335, 1733.954] Mpc/h


Splitted samples are here:

	DR12v4-CMASS/xyzw.binsplitted/
		
		data.tar.gz
			DR12v4, CMASS, in Om=0.26 LCDM. 
			columns: x, y, z, weight (wfail*wfkp*wsys)
			splitted into 3 bins

		J08*.tar.gz
			4 Mocks from HR4 simulation, in Om=0.26 LCDM
			applyint a mass-cut to have the same number density to data 
				warning: the mock has a larger galaxy bias than data
			two sets: having RSD, without RSD
			splitted into 3 bins
			

###################

I also suggest you to use them


	1. Lightcone mocks made from BigMDPL. Galaxy bias well treated
		https://github.com/seroto36/BigMD_lightcone

	2. PATCHY mocks 
		dowload all data from here:
			https://data.sdss.org/sas/dr12/boss/lss/dr12_multidark_patchy_mocks/
		for your convenience, I have 10 mocks, converted to xyzw using their cosmology (Om=0.3071 LCDM), splitted into bins
			DR12v4-CMASS/xyzw.binsplitted/PatchyV6C*.tar.gz


	3. If you want to test the systematics effects of mask, fiber collision (i.e. close pair) | let me upload them soon...
			complete_mocks_NGC/*.tar.gz





