# Available km-scale simulation on `qx55`

> [!NOTE] 
> Not all variables may be available. Zarr stores will be filled in as the simulation data becomes available.

Check [this page](https://digital-earths-global-hackathon.github.io/hosting/technical/data_request.html) to read about the metadata of the simulation and variable names. 

## um_glm_n2560_RAL3

* Model: Unified_Model
* Domain: glm (global)
* Configuration: RAL3
* Resolution: 5 km (zoom 10)
* Time start: `2020-01-20T00:00:00`
* Time end: `2021-04-01T00:00:00`
* Available frequencies: `PT1H` (2d variables) and `PT3H` (3d variables)
* Zoom: `1` to `10`

Location and list of variables (for each zoom level):
<details>
  <summary>Expand list</summary>
  
```bash
/g/data/qx55/uk_node/
├── glm.n2560_RAL3p3
│   ├── data.healpix.PT1H.z*.zarr
│   │   ├── cell
│   │   ├── clivi
│   │   ├── clt
│   │   ├── clwvi
│   │   ├── crs
│   │   ├── hflsd
│   │   ├── hfssd
│   │   ├── huss
│   │   ├── pr
│   │   ├── prs
│   │   ├── prw
│   │   ├── ps
│   │   ├── psl
│   │   ├── rlds
│   │   ├── rldscs
│   │   ├── rlut
│   │   ├── rlutcs
│   │   ├── rsds
│   │   ├── rsdscs
│   │   ├── rsdt
│   │   ├── rsut
│   │   ├── rsutcs
│   │   ├── tas
│   │   ├── time
│   │   ├── ts
│   │   ├── uas
│   │   └── vas
│   ├── data.healpix.PT3H.z*.zarr
│   │   ├── cell
│   │   ├── cli
│   │   ├── clw
│   │   ├── crs
│   │   ├── hur
│   │   ├── hus
│   │   ├── pressure
│   │   ├── qg
│   │   ├── qr
│   │   ├── qs
│   │   ├── ta
│   │   ├── time
│   │   ├── ua
│   │   ├── va
│   │   ├── wa
│   │   └── zg

```
</details>

## icon_d3hp003

* Model: ICON-ESM
* Domain: glm (global)
* Resolution: 2.5 km (zoom 11)
* Time start: `2020-01-02T00:00:00`
* Time end: `2021-03-01T00:00:00`
* Available frequencies:
  * Mean values: `P1D`, `PT6H` and `PT3H` 
  * Point (instantaneous): `P1D`, `PT12`, `PT6H` and `PT3H` (available variables changes for each frequency)
* Zoom: `0` to `11`

Location and list of variables (for each zoom level):

<details>
  <summary>Expand list</summary>
  
```bash
/g/data/qx55/german_node/
├── d3hp003.zarr
    ├── [P1D, PT3H, PT6H]_mean_z*_atm.zarr
    │   ├── clivi
    │   ├── clt
    │   ├── clwvi
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── hfls
    │   ├── hfss
    │   ├── hur
    │   ├── hus
    │   ├── hydro_fract_snow_box
    │   ├── hydro_weq_snow_box
    │   ├── hydro_wtr_soil_sl_box
    │   ├── o3vi
    │   ├── pr
    │   ├── pres_msl
    │   ├── pres_sfc
    │   ├── pressure
    │   ├── prls
    │   ├── prw
    │   ├── qall
    │   ├── qv2m
    │   ├── rlds
    │   ├── rldscs
    │   ├── rlus
    │   ├── rlut
    │   ├── rlutcs
    │   ├── rsds
    │   ├── rsdscs
    │   ├── rsdt
    │   ├── rsus
    │   ├── rsuscs
    │   ├── rsut
    │   ├── rsutcs
    │   ├── sic
    │   ├── soil_level
    │   ├── tas
    │   ├── tauu
    │   ├── tauv
    │   ├── temp
    │   ├── tend_egpdynvi
    │   ├── tend_eincldvi
    │   ├── tend_eindynvi
    │   ├── tend_einradvi
    │   ├── tend_eintmxvi
    │   ├── tend_ekhdynvi
    │   ├── tend_ekhtmxvi
    │   ├── tend_ekvdynvi
    │   ├── time
    │   ├── ts
    │   ├── u
    │   ├── uas
    │   ├── v
    │   ├── vas
    │   ├── vor
    │   ├── wa_phy
    │   └── z_mc
    ├── P1D_point_z*_atm.zarr
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── hur
    │   ├── hus
    │   ├── pr
    │   ├── pres_msl
    │   ├── pressure
    │   ├── qall
    │   ├── rlut
    │   ├── rsut
    │   ├── temp
    │   ├── time
    │   ├── ts
    │   ├── u
    │   ├── uas
    │   ├── v
    │   ├── vas
    │   ├── vor
    │   ├── wa_phy
    │   └── z_mc
    ├── PT12H_point_z*_atm.zarr
    │   ├── crs
    │   ├── orog
    │   ├── sftgif
    │   ├── sftlf
    │   └── time
    ├── PT1H_point_z*_atm.zarr
    │   ├── crs
    │   ├── pr
    │   ├── pres_msl
    │   ├── rlut
    │   ├── rsut
    │   ├── time
    │   ├── ts
    │   ├── uas
    │   └── vas
    ├── PT3H_point_z*_atm.zarr
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── pr
    │   ├── pres_msl
    │   ├── pressure
    │   ├── rlut
    │   ├── rsut
    │   ├── time
    │   ├── ts
    │   ├── uas
    │   ├── vas
    │   └── vor
    ├── PT6H_point_z*_atm.zarr
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── hur
    │   ├── hus
    │   ├── pr
    │   ├── pres_msl
    │   ├── pressure
    │   ├── qall
    │   ├── rlut
    │   ├── rsut
    │   ├── temp
    │   ├── time
    │   ├── ts
    │   ├── u
    │   ├── uas
    │   ├── v
    │   ├── vas
    │   ├── vor
    │   ├── wa_phy
    │   └── z_mc
```
</details>


