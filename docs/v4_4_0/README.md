# DUNE DAQ Data Formats offline version:  dunedaqdataformats

- This repository contains the current and all previous versions of daqdataformats from https://github.com/dune-daq/daqdataformats

- version v4_4_0 gets its name from the DUNE DAQ release made in advance of ProtoDUNE running in April 2024.  It actually uses code from daqdataformats v3.7.0

- Update August 21, 2024:  there are non-breaking changes in DUNE DAQ fddaq v4.4.4, which corresponds to daqdataformats v3.7.1.  These have simply been merged in to
  this repository without increasing the version number of the interally versioned directories, so it stays at v4_4_0 internally, but the UPS product version is
  incremented to v4_4_4.

- remaining documentation is copied from https://github.com/dune-daq/daqdataformats v3.7.0

- This repository contains raw data bitfields and utilities used to decode them
- This repository also contains classes which are generated within the DAQ and intended to be persisted to disk and read by Offline code.

The following are brief descriptions of the various structs in this package, including links to fuller, field-by-field descriptions:

----------

**Fragment**: the data fragment interface, representing the data response of one part of the detector (TPC link, etc.) to a dataflow `DataRequest` message. Contains a `FragmentHeader` and the data payload.

**FragmentHeader**: data-about-the-data, e.g. source, run number, trigger timestamp, etc.

[FragmentHeader description](FragmentHeaderV4.md)

---------------

**TriggerRecordHeaderData**: An assortment of information about a trigger. Trigger timestamp, trigger type, etc.

[TriggerRecordHeaderData description](TriggerRecordHeaderDataV3.md)

**TriggerRecordHeader**: contains an instance of `TriggerRecordHeaderData` and a set of component requests

**TriggerRecord**: contains an instance of `TriggerRecordHeader` and a set of fragments

---------------

[SourceID description](SourceIDV2.md)

---------------

[ComponentRequest description](ComponentRequestV2.md)

--------------


### API Diagrams

Common dataformat classes:
![Class Diagrams](https://github.com/DUNE-DAQ/daqdataformats/raw/develop/docs/daqdataformats-common.png)

Fragment classes:
![Class Diagrams](https://github.com/DUNE-DAQ/daqdataformats/raw/develop/docs/daqdataformats-fragment.png)

TriggerRecord classes:
![Class Diagrams](https://github.com/DUNE-DAQ/daqdataformats/raw/develop/docs/daqdataformats-record.png)

TimeSlice classes:
![Class Diagrams](https://github.com/DUNE-DAQ/daqdataformats/raw/develop/docs/daqdataformats-slice.png)