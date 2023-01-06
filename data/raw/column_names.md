# Column Descriptions

All column descriptions are based off of the descriptions present in the [NASA Exoplanet Archive - Cumulative Kepler Objects of Interest Documentation](https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html). Note that some column descriptions can be found in the [NASA Exoplanet Archive - Threshold Crossing Event Documentation](https://exoplanetarchive.ipac.caltech.edu/docs/API_tce_columns.html) instead. Column descriptions from the Kepler table begin with "koi," while column descriptions from the Threshold Crossing table begin with "tce."

The column name in the project data is given first, with the Exoplanet Archive documentation equivalent given in parentheses. Columns created during analysis have secondary alias.

<ul>
    <li>`koi_name` (kepoi_name): A number used to identify and track a Kepler Object of Interest (KOI).</li>
    <li>`false_positive_type` (koi_comment): A description of the reason why an object's disposition has been given as false positive.</li>
    <li>`disposition` (koi_disposition): The category of this KOI from the Exoplanet Archive. Current values are CANDIDATE, FALSE POSITIVE, NOT DISPOSITIONED or CONFIRMED.</li>
    <li>`fp_not_transit` (koi_fpflag_nt): Flag denoting a KOI whose light curve is not consistent with that of a transiting planet.</li>
    <li>`fp_stellar_eclipse` (koi_fpflag_ss): Flag denoting a KOI that is observed to have a significant secondary event, transit shape, or out-of-eclipse variability, which indicates that the transit-like event is most likely caused by an eclipsing binary.</li>
    <li>`fp_centroid_offset` (koi_fpflag_co): Flag denoting the source of the signal is from a nearby star, as inferred by measuring the centroid location of the image both in and out of transit, or by the strength of the transit signal in the target's outer (halo) pixels as compared to the transit signal from the pixels in the optimal (or core) aperture.</li>
    <li>`fp_contamination` (koi_fpflag_ec): Flag denoting the KOI shares the same period and epoch as another object and is judged to be the result of flux contamination in the aperture or electronic crosstalk.</li>
    <li>`classification`: Column denoting whether KOI is a confirmed planet (0), or one of the above four false positives (1-4).</li>
    <li>`num_of_objects_around_star` (koi_count): The number of Kepler Objects of Interest present around the observed star.</li>
    <li>`right_ascension` (ra): The right ascension of the KOI relative to the point of observation. This is part of the ascension/declination coordinate system.</li>
    <li>`declination` (dec): The declination of the KOI relative to the point of observation. This is part of the ascension/declination coordinate system.</li>
    <li>`g_band_mag` (koi_gmag): The magnitude of observed light from the star in the "green" wavelength band (~464nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`r_band_mag` (koi_rmag): The magnitude of observed light from the star in the "red" wavelength band (~658nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`i_band_mag` (koi_imag): The magnitude of observed light from the star in the "infrared" wavelength band (~806nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`z_band_mag` (koi_zmag): The magnitude of observed light from the star in the "beyond-infrared" wavelength band (~900nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`j_band_mag` (koi_jmag): The magnitude of observed light from the star in "J" wavelength band from 2MASS (~1220nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`h_band_mag` (koi_hmag): The magnitude of observed light from the star in "H" wavelength band from 2MASS (~1630nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`k_band_mag` (koi_kmag): The magnitude of observed light from the star in "K" wavelength band from 2MASS (~2190nm). [Wikipeda - Photometric System](https://en.wikipedia.org/wiki/Photometric_system)</li>
    <li>`kepler_band_mag` (koi_kepmag): The Kepler band magnitude of observed light from the star. [Estimating Kepler Magnitudes](https://nexsci.caltech.edu/workshop/2012/keplergo/CalibrationZeropoint.shtml)</li>
    <li>`num_of_transits` (koi_num_transits): The number of expected or partially observed transits of the KOI within the searched light curve.</li>
    <li>`max_single_event_stat` (koi_max_sngle_ev): The maximum calculated single event statistic of observed Threshold-Crossing Events (TCEs) of the KOI.</li>
    <li>`max_multi_event_stat` (koi_max_mult_ev): The maximum calculated multiple event statistic of observed TCEs of the KOI.</li>
    <li>`odd_even_depth_stat` (tce_bin_oedp_sig): The number of standard deviations from equal depth between odd and even transits.</li>
    <li>`limb_dark_co1` (koi_ldm_coeff1): One of 4 limb-darkening coefficients used to measure the intensity of a star as a function of angle.</li>
    <li>`limb_dark_co2` (koi_ldm_coeff2): One of 4 limb-darkening coefficients used to measure the intensity of a star as a function of angle.</li>
    <li>`limb_dark_co3` (koi_ldm_coeff3): One of 4 limb-darkening coefficients used to measure the intensity of a star as a function of angle.</li>
    <li>`limb_dark_co4` (koi_ldm_coeff4): One of 4 limb-darkening coefficients used to measure the intensity of a star as a function of angle.</li>
    <li>`transit_signal_to_noise` (koi_model_snr): Transit signal to noise ratio. Transit depth normalized by the mean uncertainty in flux during transits.</li>
    <li>`planet_radius_earth` (koi_prad): Radius of the KOI in Earth radii.</li>
    <li>`orbit_semimajor_axis` (koi_sma): Half of the long axis of the KOI's orbit. For a circular orbit, this corresponds to the distance from the star.</li>
    <li>`impact` (koi_impact): The sky-projected distance between the center of the stellar disc and the center of the planet disc at conjunction, normalized by the stellar radius.</li>
    <li>`transit_duration` (koi_duration): Duration of observed transit in Earth hours.</li>
    <li>`transit_depth` (koi_depth): The fraction of stellar flux lost at the minimum of the planetary transit in parts per million.</li>
    <li>`orbital_period` (koi_period): The interval between consecutive planetary transits in Earth days.</li>
    <li>`planet_star_radius_ratio` (koi_ror): The planet radius divided by the stellar radius.</li>
    <li>`planet_star_distance_radius` (koi_dor): The distance between the planet and the star at mid-transit divided by the stellar radius. For a circular orbit, the distance at mid-transit is the semi-major axis of the planetary orbit.</li>
    <li>`inclination` (koi_incl): The angle between the plane of the sky (perpendicular to the line of sight) and the orbital plane of the planet candidate in degrees.</li>
    <li>`planet_temp` (koi_teq): Approximation for the temperature of the planet in degrees Kelvin.</li>
    <li>`star_temp` (koi_steff): The photospheric temperature of the star.</li>
    <li>`star_surface_gravity (koi_slogg): The base-10 logarithm of the acceleration due to gravity at the surface of the star in cm/s^2.</li>
    <li>`star_metallicity` (koi_smet): The base-10 logarithm of the Fe to H ratio at the surface of the star, normalized by the solar Fe to H ratio.</li>
    <li>`star_radius` (koi_srad): The photospheric radius of the star in Sol radii.</li>
    <li>`flux_weight_offset_sig` (koi_fwm_stat_sig): Indicates whether there is a statistically significant flux-weighted offset between in-transit and out-of-transit images.</li>
    <li>`centroid_right_ascension` (koi_fwm_sra): The Right Ascension (J2000) of the location of the transiting object calculated from the flux-weighted centroids in hours.</li>
    <li>`centroid_declination` (koi_fwm_sdec): The Declination (J2000) of the location of the transiting object calculated from the flux-weighted centroids in degrees.</li>
    <li>`centroid_star_right_ascension_offset` (koi_fwm_srao): The RA (J2000) flux-weighted centroid shift in seconds.</li>
    <li>`centroid_star_declination_offset` (koi_fwm_sdeco): The Dec (J2000) flux-weighted centroid shift arcseconds.</li>
    <li>`planet_star_right_ascension_offset` (koi_fwm_prao): The calculated Right Ascension offset of the transiting or eclipsing object from the KIC location of the target star in seconds.</li>
    <li>`planet_star_declination_offset` (koi_fwm_pdeco): The calculated Declination offset of the transiting or eclipsing object from the KIC location of the target star in arcseconds.</li>
    <li>`angular_offset_right_ascension` (koi_dicco_mra): The angular offset in the RA (J2000) direction between the best-fit PRF centroids from the Out-Of-Transit image and the Difference Image by averaging the weighted single-quarter measurements in arcseconds.</li>
    <li>`angular_offset_declination` (koi_dicco_mdec): The angular offset in the Dec (J2000) direction between the best-fit PRF centroids from the Out-Of-Transit image and the Difference Image by averaging the weighted single-quarter measurements in arcseconds.</li> 
    <li>`angular_offset_sky` (koi_dicco_msky): The angular offset on the plane of the sky between the best-fit PRF centroids from the Out-Of-Transit image and the Difference Image by averaging the weighted single-quarter measurements in arcseconds.</li>
    <li>`insolation_flux` (koi_insol): Insolation flux is another way to give the equilibrium temperature in Earth flux.</li>
    <li>`star_density` (koi_srho): Fitted stellar density in g/cm^3.</li>
    <li>`abs_gr_diff`: The absolute difference between g- and r-band spectrums.</li>
    <li>`abs_gi_diff`: The absolute difference between g- and i-band spectrums.</li>
    <li>`abs_gz_diff`: The absolute difference between g- and z-band spectrums.</li>
    <li>`abs_ri_diff`: The absolute difference between r- and i-band spectrums.</li>
    <li>`abs_rz_diff`: The absolute difference between r- and z-band spectrums.</li>
    <li>`abs_iz_diff`: The absolute difference between i- and z-band spectrums.</li>
    <li>`abs_jh_diff`: The absolute difference between J- and H-band spectrums.</li>
    <li>`abs_jk_diff`: The absolute difference between J- and K-band spectrums.</li>
    <li>`abs_hk_diff`: The absolute difference between H- and K-band spectrums.</li>
</ul>