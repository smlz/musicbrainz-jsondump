# Export Album Data from MusicBrainz

The code can be found in this notebook: [Notebook](Notebook.ipynb)

## Installation

```
mkdir musicbrainz-jsondump
virtualenv -p /usr/bin/python3.5 musicbrainz-jsondump-env
cd musicbrainz-jsondump
pip install notebook SQLAlchemy psycopg2 PyLyrics
```

### MusicBrainz-VM

Get it from here:
https://musicbrainz.org/doc/MusicBrainz_Server/Setup

For the VM do:
* Add a NAT-port mappint from 6543 to 5432
* Set listen_address to '*' in /etc/postgresql/9.3/main/postgresql.conf
* Restart PostgreSQL (service postgresql restart)
