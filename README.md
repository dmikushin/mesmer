# MESMER

## Modular Earth System Model Emulator with spatially Resolved output

## Building

Prerequisites for Ubuntu 20.04:

```
apt install apt-file git python3 python3-venv libproj-dev proj-data proj-bin libgeos-dev libgdal-dev
```

Prerequired Python packages:

```
pip3 install -r requirements.txt
```

In case of GDAL error, note that GDAL Python bindings must correspond to the actual binary package installed in the system. The following command manages the exact correspondence:

```
pip3 install GDAL==$(gdal-config --version) --global-option=build_ext --global-option="-I/usr/include/gdal"
```

Finally, install the package itself:

```
python3 setup.py install
```

##  Citing MESMER

Scientific publications using MESMER should cite the following publication:

Beusch, Lea, Lukas Gudmundsson, and Sonia I. Seneviratne, 2020: Emulating Earth system
model temperatures with MESMER: from global mean temperature trajectories to
grid-point-level realizations on land. Earth Syst. Dynam., 11, 139–159, 2020,
https://doi.org/10.5194/esd-11-139-2020

## License

Copyright (c) 2021 ETH Zurich, MESMER contributors listed in AUTHORS.

MESMER is free software; you can redistribute it and/or modify it under the terms of the
GNU General Public License as published by the Free Software Foundation, version 3  or
(at your option) any later version.

MESMER is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR
PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with MESMER. If
not, see https://www.gnu.org/licenses/.

The full list of code contributors can be found in AUTHORS or on
[github.com/contributors](https://github.com/MESMER-group/mesmer/graphs/contributors).
