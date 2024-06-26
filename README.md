# dunedaqdataformats
Offline-versioned copies of DUNE-DAQ/daqdataformats

This repository contains versioned copies of header files used to define the data formats used by the DUNE DAQ.  Due to evolution of the formats and the need for the DUNE Offline to support reading and processing of all current and older data, all versions of these classes need to be available to all offline jobs at any time.  ROOT provides tools for automatically migrating from one version of a class to another when reading data from files, but HDF5 does not.  This repository therefore contains directories labeled by version number to maintain each version of the header files.

Version v4_4_0 gets its name from the DUNE DAQ release made in advance of ProtoDUNE running in April 2024.  It actually uses code from daqdataformats v3.7.0

Original files can be found here.

https://github.com/dune-daq/daqdataformats

HD and VD coldbox data have been collected with
dunedaqdataformats v3_3_3-formatted data, and so
this is the first version that is included in the
preservation list.  v3_4_1 is the first version
of dunedaqdataformats to introduce the versioning
scheme.


## Copyright and Licensing
Copyright © 2023 FERMI NATIONAL ACCELERATOR LABORATORY for the benefit of the DUNE Collaboration.

This repository, and all software contained within, except where noted within the individual source files, is licensed under
the Apache License, Version 2.0 (the "License"); you may not use this
file except in compliance with the License. You may obtain a copy of
the License at

    http://www.apache.org/licenses/LICENSE-2.0

Copyright is granted to FERMI NATIONAL ACCELERATOR LABORATORY on behalf
of the Deep Underground Neutrino Experiment (DUNE). Unless required by
applicable law or agreed to in writing, software distributed under the
License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied. See the License for
the specific language governing permissions and limitations under the
License.
