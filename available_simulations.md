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
* [More information](https://github.com/digital-earths-global-hackathon/hk25/blob/main/content/models/um.md)

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
  * Mean values: `P1D` and `PT3H` 
  * Point (instantaneous): `P1D`, `PT3H` and `PT1H` (available variables changes for each frequency)
* Zoom: `5` to `11
* [More information](https://github.com/digital-earths-global-hackathon/hk25/blob/main/content/models/icon.md)

Location and list of variables (for each zoom level):

<details>
  <summary>Expand list</summary>
  
```bash
/g/data/qx55/german_node/
└── d3hp003.zarr
    ├── P1D_mean_z*_atm.zarr
    │   ├── clivi
    │   ├── clt
    │   ├── clwvi
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── hflsd
    │   ├── hfssd
    │   ├── hur
    │   ├── hus
    │   ├── huss
    │   ├── mrso
    │   ├── o3vi
    │   ├── orog
    │   ├── pr
    │   ├── pressure
    │   ├── pressure_rva
    │   ├── prs
    │   ├── prw
    │   ├── ps
    │   ├── psl
    │   ├── qall
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
    │   ├── rva
    │   ├── sftgif
    │   ├── sftlf
    │   ├── siconc
    │   ├── sncvfa
    │   ├── soil_level
    │   ├── swe
    │   ├── ta
    │   ├── tas
    │   ├── tauu
    │   ├── tauv
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
    │   ├── ua
    │   ├── uas
    │   ├── va
    │   ├── vas
    │   ├── wa
    │   └── zg
    ├── P1D_point_z*_atm.zarr
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── hur
    │   ├── hus
    │   ├── orog
    │   ├── pr
    │   ├── pressure
    │   ├── pressure_rva
    │   ├── psl
    │   ├── qall
    │   ├── rlut
    │   ├── rsut
    │   ├── rva
    │   ├── sftgif
    │   ├── sftlf
    │   ├── ta
    │   ├── time
    │   ├── ts
    │   ├── ua
    │   ├── uas
    │   ├── va
    │   ├── vas
    │   ├── wa
    │   └── zg
    ├── PT1H_point_z*_atm.zarr
    │   ├── crs
    │   ├── orog
    │   ├── pr
    │   ├── psl
    │   ├── rlut
    │   ├── rsut
    │   ├── sftgif
    │   ├── sftlf
    │   ├── time
    │   ├── ts
    │   ├── uas
    │   └── vas
    ├── PT3H_mean_z*_atm.zarr
    │   ├── clivi
    │   ├── clt
    │   ├── clwvi
    │   ├── crs
    │   ├── hflsd
    │   ├── hfssd
    │   ├── huss
    │   ├── mrso
    │   ├── o3vi
    │   ├── orog
    │   ├── pr
    │   ├── prs
    │   ├── prw
    │   ├── ps
    │   ├── psl
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
    │   ├── sftgif
    │   ├── sftlf
    │   ├── siconc
    │   ├── sncvfa
    │   ├── soil_level
    │   ├── swe
    │   ├── tas
    │   ├── tauu
    │   ├── tauv
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
    │   ├── uas
    │   └── vas
    ├── PT3H_point_z*_atm.zarr
    │   ├── crs
    │   ├── egpvi
    │   ├── einvi
    │   ├── ekhvi
    │   ├── ekvvi
    │   ├── orog
    │   ├── pr
    │   ├── pressure
    │   ├── pressure_rva
    │   ├── psl
    │   ├── rlut
    │   ├── rsut
    │   ├── rva
    │   ├── sftgif
    │   ├── sftlf
    │   ├── time
    │   ├── ts
    │   ├── uas
    │   └── vas
```
</details>


