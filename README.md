# CIF CIPC Channels

LabVIEW channels that pass tag and FIFO data between plugins over NI CIPC (circular interprocess communication). This package was split out of [CIF Channels Core](https://github.com/CIF-Foundation/CIF_Channels_Core).

Channel classes inherit from `CIF_CIPC_Chn.lvclass`.

## Channels

**Tags**

| Class | Data |
| --- | --- |
| `CIF_CIPC_Chn_Double` | Double |
| `CIF_CIPC_Chn_I64` | I64 |
| `CIF_CIPC_Chn_U64` | U64 |
| `CIF_CIPC_Chn_String` | String |

**FIFOs**

| Class | Data |
| --- | --- |
| `CIF_CIPC_Universal` | Universal |
| `CIF_CIPC_Fifo_U8` | U8 array |
| `CIF_CIPC_Fifo_DAQ` | DAQ |
| `CIF_CIPC_CAN` | CAN |
| `CIF_CIPC_L2Enet` | Layer 2 Ethernet |

## Installation

Install these packages first:

- [CIF Channels Core](https://github.com/CIF-Foundation/CIF_Channels_Core) (`CIF_Foundation_lib_CIF_Channels`) 3.1.0.3 or later
- [CIF Utilities](https://github.com/CIF-Foundation/CIF_Utilities) (`CIF_Foundation_lib_CIF_Utilities`) 4.18.3.2 or later
- [CIF CIPC](https://github.com/CIF-Foundation/CIF_NI_CIPC) (`CIF_Foundation_lib_NI_CIPC`) 2.0.0.1 or later

Build or install this package from [`VIPM/CIF_CIPC_Channels.vipb`](VIPM/CIF_CIPC_Channels.vipb). The VIPM package name is `CIF_Foundation_lib_CIF_CIPC_Channels`.

Requires LabVIEW 2021 (64-bit) or later.

After installation, VIs are on the LabVIEW palette at:

`Functions » CIF » Channels » CIPC`

That palette has **Tags** and **CIPC FIFO** subpalettes.

## Repository Layout

| Path | Description |
| --- | --- |
| `src/CIPC_Channels/` | LabVIEW source for the CIPC channel classes, accessors, and tests |
| `VIPM/` | VI Package Manager build specification |
| `LICENSE` | Apache License 2.0 |

## License

Copyright 2026 CIF Foundation

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this project except in compliance with the License. You may obtain a copy of the License at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

The full license text is in [`LICENSE`](LICENSE).
