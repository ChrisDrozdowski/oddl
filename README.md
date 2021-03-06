# oddl (OpeNDAP Downloader)

oddl (OpeNDAP Downloader): a GUI-based Python app for downloading and saving netCDF data via OpeNDAP.

*Note: This is an experimental project.*

Installation:
```
pip install oddl
```

The app can be run from the command line via: `oddl`

Or you can run it via script via:
```
from oddl import run

run()
```

## Authors

* [Chris Drozdowski](https://github.com/chrisdrozdowski)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Examples/requirements of OpeNDAP Requests

#### Example of no authorization OpeNDAP request

Base URL: http://test.opendap.org/opendap/data/nc/sst.mnmean.nc.gz

Auth Type: "none"

OpenID/Auth URL: not required

User ID: not required

Password: not required


#### Example of URS NASA EARTHDATA OpeNDAP request

*Requires URS NASA EARTHDATA account for access. Must accept EULA(s) and allow App on your account. App means and is based on request URL*

Base URL: https://goldsmr5.gesdisc.eosdis.nasa.gov:443/opendap/MERRA2_MONTHLY/M2IMNPANA.5.12.4/2019/MERRA2_400.instM_3d_ana_Np.201901.nc4

Auth Type: "URS"

OpenID/Auth URL: not required

User ID: required

Password: required


#### Example of Earth System Grid Federation (ESGF) OpeNDAP request

*Requires Earth System Grid Federation (ESGF) account for access.*

Base URL: http://esgf-data.ucar.edu/thredds/dodsC/esg_dataroot/CMIP6/CMIP/NCAR/CESM2/historical/r10i1p1f1/Amon/tas/gn/v20190313/tas_Amon_CESM2_historical_r10i1p1f1_gn_200001-201412.nc

Auth Type: "ESGF"

OpenID/Auth URL: required

User ID: not required (but required if your openid contains contains the string ```ceda.ac.uk```, it is required)

Password: required


#### Example of CAS OpeNDAP request

*Research needs to be done into a valid example and info about account*

Base URL: No example yet

Auth Type: "CAS"

OpenID/Auth URL: required

User ID: required

Password: required
