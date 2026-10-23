# NM_Database

LabVIEW library for SQL Server communication: detects installed SQL/OLE DB drivers,
manages database connections and builds connection strings.

## Features
- Check SQL Server availability (`SQL_CHECK-Server.vi`)
- Detect installed SQL/OLE DB drivers (`SQL_Search_Drivername.vi`)
- Create connection strings and connect via MSOLEDBSQL (`SQL_Connect_MSOLEDBSQL.vi`)
- Convert date/time values to SQL strings (`SQL_DateTime_SQLstring.vi`)

## Requirements
- LabVIEW 2024 Q3 (24.3) or later
- VIPM to install the package
- Microsoft OLE DB Driver for SQL Server (MSOLEDBSQL) for connections

## Installation
Download the `.vip` file from the [Releases](../../releases) page and open it with VIPM.

## Repository layout
| Folder | Content |
| --- | --- |
| `source/` | LabVIEW source code (`DB-Tool.lvlib` and VIs) |
| `package/` | VIPM package specification (`NM_Database.vipb`) |
| `NM_Database.lvproj` | LabVIEW project |

## Build
Open `package/NM_Database.vipb` in the VI Package Builder and build the package.
Attach the resulting `.vip` to a GitHub release (do not commit it).

## License
MIT, see [LICENSE](LICENSE). Provided "as is", without warranty. Free, non-commercial publication.

## Security
See [SECURITY.md](SECURITY.md).
