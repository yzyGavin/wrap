# Kinematic aircraft performance database

As part of Open Aircraft Performance model, the WRAP database provides operational performance, flight envelopes of aircraft performance parameters. ADS-B data are use for model construction. Detailed methods and model description can be found in the paper.

------

## Parameters

The parameters are defined by flight phases. The method to extract these parameters are define in the paper.

##### Takeoff

- liftoff speed (``to_v_lof``)
- takeoff distance (``to_d_tof``)
- mean takeoff acceleration (``to_acc_tof``)

#### Initial climb:
- cutoff altitude (``1500 ft``)
- calibrated airspeed (``ic_va_avg``)
- vertical rate (``ic_vh_avg``)

#### Climb:
- range to the top of climb (``cl_d_range``)
- constant CAS crossover altitude (``cl_h_cas_const``)
- constant CAS (``cl_v_cas_const``)
- vertical rate during constant CAS climb (``cl_vz_avg_pre_cas``)
- constant Mach climb crossover altitude (``cl_h_mach_const``)
- constant Mach number (``cl_v_mach_const``)
- vertical rate during constant Mach climb (``cl_vz_avg_mach_const``)
- vertical rate before constant CAS climb (``cl_vz_avg_pre_cas``)

#### Cruise:
- cruise range (``cr_d_range``)
- nominal cruise altitude (``cr_h_mean``)
- maximum cruise altitude (``cr_h_max``)
- nominal cruise Mach number (``cr_v_mach_mean``)
- maximum cruise Mach number (``cr_v_mach_max``)

#### Descent:
- range from the top of descent (``de_d_range``)
- constant Mach number (``de_v_mach_const``)
- constant Mach descent crossover altitude (``de_h_mach_const``)
- vertical rate during constant Mach descent (``de_vz_avg_mach_const``)
- constant CAS (``de_v_cas_const``)
- constant CAS crossover altitude (``de_h_cas_const``)
- vertical rate during constant CAS descent (``de_vz_avg_cas_const``)
- vertical rate after constant CAS descent (``de_vz_avg_after_cas``)

#### Final approach:
- cutoff altitude (``1500 ft``)
- calibrated airspeed (``fa_va_avg``)
- vertical rate (``fa_vh_avg``)

#### Landing:
- touchdown speed (``ld_v_app``)
- breaking distance (``ld_d_brk``)
- mean breaking deceleration (``ld_acc_brk``)

------

## Supporting Aircraft types
  * Airbus
    * A319, A320, A321, A332, A333, A343, A388
  * Boeing
    * B737, B738, B739, B744, B752, B763, B77W, B788, B789
  * Other
    * E190
