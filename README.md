# DemiGaze
A host connection logging and database aggregation tool. Uses ipinfo.io, whois, and the socket api

This will get more mature as it goes along, but it is a neat concept.

TODO:

- Improve schema for results on all data.
- Improve threading for concurrent scanning for connections while scanning hosts
- Improve overlap areas
- Implement host url determination from host info
- Implement root domain determination if possible for the host
- Implement functionality for Linux and other OSes

## Usage

Please see requirements.txt

Install [`whois`](https://learn.microsoft.com/en-us/sysinternals/downloads/whois) on your system and place it within path or the directory where DemiGaze is located.

```
$ mkdir temp
$ python DemiGaze.py
Performing WHOIS lookups for remote IPs...
280 IPs catalogued already
280 IPs catalogued now. 0 new entries
...
...
...
Performing WHOIS lookups for remote IPs...
280 IPs catalogued already
280 IPs catalogued now. 0 new entries
```

## Modification

There will eventually be a tunables file.

```python
output_dir = os.path.abspath('.' + os.path.sep + 'temp')
dbname = 'host-lookups.db'
```

## Installation

Haven't made one yet