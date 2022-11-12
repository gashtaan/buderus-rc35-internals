# Parameter tables

Devices connected to common EMS bus communicate with each other by exchanging various parameter tables encapsulated in **telegrams**.

Some tables belongs to **local** RC35 controller itself, other belongs to some **external** device and some are **shared** between multiple devices and broadcasted to others when device make changes in them to every device have the most recent data.

Optional number in column **interval** in the following table indicate that device is actively broadcasting/querying parameter table to/from other devices in specified time intervals (in seconds).

Tables marked as **persistent** have their parameters (in addition to RAM) backed also in built-in EEPROM memory to make them survive a restart or power outage.

> These parameter tables can be viewed/edited in hidden technician menu built into RC35 unit. It is accesible from Service/Diagnosis/Versions menu by pushing TEMP, INFO and TIME buttons at the same time and while keeping them pushed down, rotating the knob clockwise at least five times.

| Index | Owner | Data Type | Bus Device | Interval | Persistent |
|-------|-------|-----------|-------------|----------|------------|
| [0](#parameter-table-0) | external | 07 | MC10 (8) | 180 | no |
| [1](#parameter-table-1) | external | 02 | MC10 (8) | - | no |
| [2](#parameter-table-2) | external | 04 | MC10 (8) | - | no |
| [3](#parameter-table-3) | local | 1A | MC10 (8) | 60 | no |
| [4](#parameter-table-4) | external | 10 | MC10 (8) | 600 | no |
| [5](#parameter-table-5) | external | 11 | MC10 (8) | 600 | no |
| [6](#parameter-table-6) | shared | 33 | MC10 (8) | - | yes |
| [7](#parameter-table-7) | local | 35 | MC10 (8) | 60 | no |
| [8](#parameter-table-8) | external | 34 | MC10 (8) | 180 | no |
| [9](#parameter-table-9) | external | 18 | MC10 (8) | 180 | no |
| [10](#parameter-table-10) | external | 19 | MC10 (8) | 360 | no |
| [11](#parameter-table-11) | external | 1C | MC10 (8) | 1200 | no |
| [12](#parameter-table-12) | external | 14 | MC10 (8) | 120 | no |
| [13](#parameter-table-13) | shared | 15 | MC10 (8) | - | yes |
| [14](#parameter-table-14) | shared | 16 | MC10 (8) | - | yes |
| [15](#parameter-table-15) | shared | 25 | MC10 (8) | - | yes |
| [16](#parameter-table-16) | shared | 27 | MC10 (8) | - | yes |
| [17](#parameter-table-17) | external | 2A | MC10 (8) | 180 | no |
| [18](#parameter-table-18) | local | 1D | MC10 (8) | - | no |
| [19](#parameter-table-19) | external | 08 | MC10 (8) | 180 | no |
| [20](#parameter-table-20) | external | 29 | BC10 (9) | 600 | no |
| [21](#parameter-table-21) | external | 02 | BC10 (9) | - | no |
| [22](#parameter-table-22) | shared | 9B | PM10 (21) | - | yes |
| [23](#parameter-table-23) | external | 9C | PM10 (21) | 360 | no |
| [24](#parameter-table-24) | external | 02 | PM10 (21) | - | no |
| [25](#parameter-table-25) | local | A0 | PM10 (21) | - | no |
| [26](#parameter-table-26) | shared | 9B | PM10 (17) | - | yes |
| [27](#parameter-table-27) | external | 9C | PM10 (17) | 360 | no |
| [28](#parameter-table-28) | local | 9D | PM10 (17) | 60 | no |
| [29](#parameter-table-29) | external | 02 | PM10 (17) | - | no |
| [30](#parameter-table-30) | local | A0 | PM10 (17) | - | no |
| [31](#parameter-table-31) | shared | 96 | SM10 (48) | - | yes |
| [32](#parameter-table-32) | external | 97 | SM10 (48) | 360 | no |
| [33](#parameter-table-33) | external | 02 | SM10 (48) | - | no |
| [34](#parameter-table-34) | local | A0 | SM10 (48) | - | no |
| [35](#parameter-table-35) | external | 02 | RC20 HC1 (24) | - | no |
| [36](#parameter-table-36) | external | AF | RC20 HC1 (24) | 240 | no |
| [37](#parameter-table-37) | external | 02 | RC20 HC2 (25) | - | no |
| [38](#parameter-table-38) | external | AF | RC20 HC2 (25) | 240 | no |
| [39](#parameter-table-39) | external | 02 | RC20 HC3 (26) | - | no |
| [40](#parameter-table-40) | external | AF | RC20 HC3 (26) | 240 | no |
| [41](#parameter-table-41) | external | 02 | RC20 HC4 (27) | - | no |
| [42](#parameter-table-42) | external | AF | RC20 HC4 (27) | 240 | no |
| [43](#parameter-table-43) | external | 02 | RC20 HC5 (28) | - | no |
| [44](#parameter-table-44) | external | AF | RC20 HC5 (28) | 240 | no |
| [45](#parameter-table-45) | - | - | - | - | yes |
| [46](#parameter-table-46) | shared | AA | MM10 HC2 (33) | - | yes |
| [47](#parameter-table-47) | external | AB | MM10 HC2 (33) | 360 | no |
| [48](#parameter-table-48) | local | AC | MM10 HC2 (33) | 60 | no |
| [49](#parameter-table-49) | external | 02 | MM10 HC2 (33) | - | no |
| [50](#parameter-table-50) | local | A0 | MM10 HC2 (33) | - | no |
| [51](#parameter-table-51) | shared | AA | MM10 HC3 (34) | - | yes |
| [52](#parameter-table-52) | external | AB | MM10 HC3 (34) | 360 | no |
| [53](#parameter-table-53) | local | AC | MM10 HC3 (34) | 60 | no |
| [54](#parameter-table-54) | external | 02 | MM10 HC3 (34) | - | no |
| [55](#parameter-table-55) | local | A0 | MM10 HC3 (34) | - | no |
| [56](#parameter-table-56) | shared | AA | MM10 HC4 (35) | - | yes |
| [57](#parameter-table-57) | external | AB | MM10 HC4 (35) | 360 | no |
| [58](#parameter-table-58) | local | AC | MM10 HC4 (35) | 60 | no |
| [59](#parameter-table-59) | external | 02 | MM10 HC4 (35) | - | no |
| [60](#parameter-table-60) | local | A0 | MM10 HC4 (35) | - | no |
| [61](#parameter-table-61) | shared | AA | MM10 HC5 (36) | - | yes |
| [62](#parameter-table-62) | external | AB | MM10 HC5 (36) | 360 | no |
| [63](#parameter-table-63) | local | AC | MM10 HC5 (36) | 60 | no |
| [64](#parameter-table-64) | external | 02 | MM10 HC5 (36) | - | no |
| [65](#parameter-table-65) | local | A0 | MM10 HC5 (36) | - | no |
| [66](#parameter-table-66) | external | 02 | WM10 (19) | - | no |
| [67](#parameter-table-67) | local | 1D | WM10 (19) | - | no |
| [68](#parameter-table-68) | external | 02 | EM10 (18) | - | no |
| [69](#parameter-table-69) | local | 1D | EM10 (18) | - | no |
| [70](#parameter-table-70) | local | 02 | ANY | - | no |
| [71](#parameter-table-71) | shared | 01 | ANY | - | yes |
| [72](#parameter-table-72) | shared | 37 | ANY | - | yes |
| [73](#parameter-table-73) | shared | 06 | ANY | 60 | no |
| [74](#parameter-table-74) | local | A2 | ANY | 240 | no |
| [75](#parameter-table-75) | - | - | - | - | yes |
| [76](#parameter-table-76) | local | 12 | ANY | - | yes |
| [77](#parameter-table-77) | local | 13 | ANY | - | yes |
| [78](#parameter-table-78-83-88-93-98) | shared | 3D | ANY | - | yes |
| [79](#parameter-table-79-84-89-94-99) | local | 3E | ANY | 60 | no |
| [80](#parameter-table-80-85-90-95-100) | - | - | - | - | yes |
| [81](#parameter-table-81-86-91-96-101-103-104) | shared | 3F | ANY | - | yes |
| [82](#parameter-table-82-87-92-97-102) | shared | 42 | ANY | - | yes |
| [83](#parameter-table-78-83-88-93-98) | shared | 47 | ANY | - | yes |
| [84](#parameter-table-79-84-89-94-99) | local | 48 | ANY | 60 | no |
| [85](#parameter-table-80-85-90-95-100) | - | - | - | - | yes |
| [86](#parameter-table-81-86-91-96-101-103-104) | shared | 49 | ANY | - | yes |
| [87](#parameter-table-82-87-92-97-102) | shared | 4C | ANY | - | yes |
| [88](#parameter-table-78-83-88-93-98) | shared | 51 | ANY | - | yes |
| [89](#parameter-table-79-84-89-94-99) | local | 52 | ANY | 60 | no |
| [90](#parameter-table-80-85-90-95-100) | - | - | - | - | yes |
| [91](#parameter-table-81-86-91-96-101-103-104) | shared | 53 | ANY | - | yes |
| [92](#parameter-table-82-87-92-97-102) | shared | 56 | ANY | - | yes |
| [93](#parameter-table-78-83-88-93-98) | shared | 5B | ANY | - | yes |
| [94](#parameter-table-79-84-89-94-99) | local | 5C | ANY | 60 | no |
| [95](#parameter-table-80-85-90-95-100) | - | - | - | - | yes |
| [96](#parameter-table-81-86-91-96-101-103-104) | shared | 5D | ANY | - | yes |
| [97](#parameter-table-82-87-92-97-102) | shared | 60 | ANY | - | yes |
| [98](#parameter-table-78-83-88-93-98) | - | - | - | - | yes |
| [99](#parameter-table-79-84-89-94-99) | - | 66 | ANY | 60 | no |
| [100](#parameter-table-80-85-90-95-100) | - | - | - | - | yes |
| [101](#parameter-table-81-86-91-96-101-103-104) | - | - | - | - | yes |
| [102](#parameter-table-82-87-92-97-102) | - | - | - | - | yes |
| [103](#parameter-table-81-86-91-96-101-103-104) | shared | 38 | ANY | - | yes |
| [104](#parameter-table-81-86-91-96-101-103-104) | shared | 39 | ANY | - | yes |
| [105](#parameter-table-105) | shared | A5 | ANY | - | yes |
| [106](#parameter-table-106) | local | A3 | ANY | 60 | no |
| [107](#parameter-table-107) | external | A0 | ANY | - | no |
| [108](#parameter-table-108) | local | A1 | ANY | - | no |
| [109](#parameter-table-109) | external | 02 | RC20 (23) | - | no |
| [110](#parameter-table-110) | shared | AD | RC20 (23) | - | yes |
| [111](#parameter-table-111) | external | AE | RC20 (23) | - | no |
| [112](#parameter-table-112) | shared | A4 | ANY | - | yes |
## Parameter table 0
| Index | Size | Description |
|-------|------|-------------|
| 0 | 15 | Bit array maintained by master controller (MC10) where there is a bit for every valid bus address (8-127) that indicates the device presence on the bus. The first one (LSB) is always set, because bus address 8 is the master controller itself. |
## Parameter table 1
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Control unit type:<br/>48 - MC10<br/>54 - DBA<br/>5F - UBA-H3<br/>73 - UBA3.5<br/>79 - MCM10<br/>7B - UBA4/EMS |
| 1 | 1 | MC10 version major |
| 2 | 1 | MC10 version minor |
| 3 | 1 | Burner module type:<br/>76 - MC10/BRM10<br/>other - SAFe |
| 4 | 1 | Burner module version major |
| 5 | 1 | Burner module version minor |
| 6 | 1 ||
| 7 | 1 | UM10 version major |
| 8 | 1 | UM10 version minor |
| 9 | 1 ||
## Parameter table 2
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 | KIM number |
| 1 | 1 | KIM version |
| 2 | 1 | Flags |
| 3 | 1 | Boiler maximum output (kW) low byte  |
| 4 | 1 | Boiler minimum output (%) |
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 | Minimum ON temperature |
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 | Boiler maximum output (kW) high byte |
| 12 | 1 ||
| 13 | 1 | Flags |
| 14 | 1 | Flags |
| 15 | 1 ||
| 16 | 1 ||
| 17 | 2 ||
| 18 | 1 | flags |
## Parameter table 3
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Boiler temperature target |
| 1 | 1 | Boiler HC power target |
| 2 | 1 | Boiler DHW power target |
| 3 | 1 | 00/FF - Signal to boiler that heating will be needed soon<br/>If feature is enabled and how much time ahead is boiler signaled is configurable by parameter 105/8. |
## Parameter table 4
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 2 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 2 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 2 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 2 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 2 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
| 27 | 1 ||
| 28 | 2 ||
| 29 | 1 ||
| 30 | 1 ||
| 31 | 1 ||
| 32 | 2 ||
| 33 | 1 ||
| 34 | 1 ||
| 35 | 1 ||
| 36 | 1 ||
| 37 | 1 ||
| 38 | 2 ||
| 39 | 1 ||
| 40 | 1 ||
| 41 | 1 ||
| 42 | 2 ||
| 43 | 1 ||
| 44 | 1 ||
| 45 | 1 ||
| 46 | 1 ||
| 47 | 1 ||
| 48 | 2 ||
| 49 | 1 ||
| 50 | 1 ||
| 51 | 1 ||
| 52 | 2 ||
| 53 | 1 ||
| 54 | 1 ||
| 55 | 1 ||
| 56 | 1 ||
| 57 | 1 ||
| 58 | 2 ||
| 59 | 1 ||
| 60 | 1 ||
| 61 | 1 ||
| 62 | 2 ||
| 63 | 1 ||
| 64 | 1 ||
| 65 | 1 ||
| 66 | 1 ||
| 67 | 1 ||
| 68 | 2 ||
| 69 | 1 ||
| 70 | 1 ||
| 71 | 1 ||
| 72 | 2 ||
| 73 | 1 ||
| 74 | 1 ||
| 75 | 1 ||
| 76 | 1 ||
| 77 | 1 ||
| 78 | 2 ||
| 79 | 1 ||
## Parameter table 5
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 2 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 2 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 2 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 2 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 2 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
| 27 | 1 ||
| 28 | 2 ||
| 29 | 1 ||
| 30 | 1 ||
| 31 | 1 ||
| 32 | 2 ||
| 33 | 1 ||
| 34 | 1 ||
| 35 | 1 ||
| 36 | 1 ||
| 37 | 1 ||
| 38 | 2 ||
| 39 | 1 ||
| 40 | 1 ||
| 41 | 1 ||
| 42 | 2 ||
| 43 | 1 ||
| 44 | 1 ||
| 45 | 1 ||
| 46 | 1 ||
| 47 | 1 ||
| 48 | 2 ||
| 49 | 1 ||
## Parameter table 6
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 8 | 0 | DHW system enabled |
| 1 | 1 | -1 | 0 | -1 | DHW system installed |
| 2 | 1 | 30 | 80 | 60 | DHW desired temperature |
| 3 | 1 | -20 | -2 | -5 ||
| 4 | 1 | -1 | 0 | -1 ||
| 5 | 1 | 0 | 40 | 40 ||
| 6 | 1 | -1 | 0 | -1 | Circulation pump installed |
| 7 | 1 | 1 | 7 | 2 | Circulation pump switch ON frequency (per hour) |
| 8 | 1 | 60 | 80 | 70 | DHW disinfection temperature |
| 9 | 1 | -40 | 0 | 0 ||
| 10 | 1 | -1 | 0 | -1 ||
## Parameter table 7
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | DHW flags:<br/>bit 0 - enabled<br/>bit 1 - single charge active (reset by boiler when stopped)<br/>bit 2 - disinfection active (reset by boiler when stopped)<br/>bit 4 - day mode<br/>bit 5 - single charge requested (reset by unit when request is cancelled)<br/>bit 6 - disinfection requested |
| 1 | 1 | Circulation pump flags:<br/>bit 0 - enabled<br/>bit 1 - circulation active (reset by boiler when stopped)<br/>bit 4 - day mode<br/>bit 5 - circulation requested  |
## Parameter table 8
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | DHW target temperature |
| 1 | 2 | DHW measured temperature |
| 2 | 2 ||
| 3 | 1 | DHW flags:<br/>bit 0 - day mode<br/>bit 1 - single charge in progress |
| 4 | 1 | DHW error flags:<br/>bit 0 - sensor 1 is defect<br/>bit 1 - sensor 2 is defect<br/>bit 2 - water stays cold<br/>bit 3 - disinfection was unsuccessful |
| 5 | 1 | Circulation pump flags |
| 6 | 1 ||
| 7 | 1 ||
| 8 | 3 ||
| 9 | 3 ||
## Parameter table 9
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 2 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 2 ||
| 9 | 2 ||
| 10 | 2 ||
| 11 | 2 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 2 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 1 ||
| 19 | 2 ||
| 20 | 2 ||
| 21 | 2 ||
| 22 | 1 ||
| 23 | 2 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
## Parameter table 10
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 2 ||
| 2 | 2 ||
| 3 | 2 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 3 ||
| 7 | 3 ||
| 8 | 3 ||
| 9 | 3 ||
| 10 | 3 ||
| 11 | 2 ||
## Parameter table 11
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 3 ||
| 9 | 4 ||
| 10 | 4 ||
| 11 | 4 ||
## Parameter table 12
| Index | Size | Description |
|-------|------|-------------|
| 0 | 3 ||
## Parameter table 13
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 3 | 0 ||
| 1 | 1 | 10 | 60 | 60 ||
| 2 | 1 | 1 | 31 | 1 ||
| 3 | 1 | 1 | 12 | 1 ||
| 4 | 1 | 0 | 127 | 3 ||
## Parameter table 14
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 30 | 90 | 90 ||
| 2 | 1 | 0 | 100 | 100 ||
| 3 | 1 | -1 | 0 | 0 ||
| 4 | 1 | 2 | 15 | 6 ||
| 5 | 1 | -15 | -2 | -6 ||
| 6 | 1 | 0 | 60 | 10 ||
| 7 | 1 | 0 | 2 | 1 ||
| 8 | 1 | 0 | 61 | 5 ||
| 9 | 1 | 0 | 100 | 100 ||
| 10 | 1 | 0 | 100 | 100 ||
| 11 | 1 | 0 | 8 | 2 ||
| 12 | 1 | 2 | 15 | 8 ||
| 13 | 1 | -15 | -2 | -8 ||
| 14 | 1 | 4 | 75 | 15 ||
| 15 | 1 | 4 | 75 | 15 ||
| 16 | 1 | 4 | 75 | 15 ||
| 17 | 1 | 4 | 75 | 15 ||
| 18 | 1 | 0 | 60 | 30 ||
| 19 | 1 | 0 | 15 | 5 ||
| 20 | 1 | 0 | 10 | 4 ||
| 21 | 1 | -9 | 9 | 0 ||
| 22 | 1 | -9 | 9 | 0 ||
| 23 | 1 | 0 | 65 | 47 ||
| 24 | 1 | 30 | 90 | 40 ||
| 25 | 1 | -1 | 0 | 0 ||
| 26 | 1 | 30 | 90 | 60 ||
## Parameter table 15
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 3 | 0 ||
| 1 | 1 | 20 | 60 | 20 ||
| 2 | 1 | 0 | 2 | 0 ||
| 3 | 1 | -1 | 0 | -1 ||
| 4 | 1 | 0 | 6 | 0 ||
| 5 | 1 | 0 | 2 | 1 ||
| 6 | 1 | 0 | 2 | 0 ||
| 7 | 1 | 0 | 3 | 0 ||
| 8 | 1 | 0 | 3 | 0 ||
| 9 | 1 | -1 | 0 | -1 ||
| 10 | 1 | 0 | 2 | 0 ||
## Parameter table 16
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | 0 ||
| 1 | 1 | 20 | 60 | 20 ||
| 2 | 1 | 0 | 30 | 0 ||
| 3 | 1 | 40 | 65 | 40 ||
| 4 | 1 | 25 | 50 | 25 ||
| 5 | 1 | 2 | 12 | 2 ||
| 6 | 1 | -1 | 0 | -1 ||
| 7 | 1 | -1 | 0 | 0 ||
| 8 | 1 | -1 | 0 | -1 ||
| 9 | 1 | 0 | 50 | 0 ||
## Parameter table 17
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 2 ||
| 8 | 2 ||
| 9 | 2 ||
| 10 | 1 ||
| 11 | 2 ||
| 12 | 2 ||
| 13 | 2 ||
| 14 | 1 ||
## Parameter table 18
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
## Parameter table 19
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 2 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 2 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 2 ||
| 11 | 1 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 2 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 2 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 2 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 2 ||
| 27 | 1 ||
| 28 | 1 ||
| 29 | 1 ||
| 30 | 2 ||
| 31 | 1 ||
| 32 | 1 ||
| 33 | 1 ||
| 34 | 2 ||
| 35 | 1 ||
| 36 | 1 ||
| 37 | 1 ||
| 38 | 2 ||
| 39 | 1 ||
| 40 | 1 ||
| 41 | 1 ||
| 42 | 2 ||
| 43 | 1 ||
| 44 | 1 ||
| 45 | 1 ||
| 46 | 2 ||
| 47 | 1 ||
| 48 | 1 ||
| 49 | 1 ||
| 50 | 2 ||
| 51 | 1 ||
| 52 | 1 ||
| 53 | 1 ||
| 54 | 2 ||
| 55 | 1 ||
| 56 | 1 ||
| 57 | 1 ||
| 58 | 2 ||
| 59 | 1 ||
| 60 | 1 ||
| 61 | 1 ||
| 62 | 2 ||
| 63 | 1 ||
## Parameter table 20
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
## Parameter table 21
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 22
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | 0 ||
| 1 | 1 | -1 | 0 | 0 ||
| 2 | 1 | 0 | 20 | 5 ||
| 3 | 1 | 0 | 100 | 50 ||
| 4 | 1 | 0 | 100 | 100 ||
| 5 | 1 | 1 | 100 | 10 ||
| 6 | 1 | 0 | 100 | 10 ||
| 7 | 1 | 0 | 50 | 0 ||
## Parameter table 23
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
## Parameter table 24
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 25
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 26
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | 0 ||
## Parameter table 27
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 28
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
## Parameter table 29
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 30
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 31
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | 0 ||
| 1 | 1 | 20 | 28 | 24 ||
| 2 | 1 | 20 | 100 | 30 ||
| 3 | 1 | 1 | 30 | 10 ||
| 4 | 1 | 0 | 2 | 2 ||
| 5 | 1 | 30 | 90 | 60 ||
| 6 | 1 | 30 | 55 | 55 ||
| 7 | 1 | 7 | 30 | 10 ||
| 8 | 1 | 5 | 15 | 5 ||
| 9 | 1 | 10 | 60 | 45 ||
| 10 | 1 | 10 | 50 | 30 ||
| 11 | 1 | 5 | 30 | 15 ||
| 12 | 1 | 20 | 100 | 100 ||
| 13 | 1 | 0 | 50 | 40 ||
| 14 | 1 | 2 | 20 | 10 ||
## Parameter table 32
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 2 ||
| 3 | 1 ||
| 4 | 2 ||
| 5 | 1 ||
| 6 | 3 ||
| 7 | 1 ||
| 8 | 1 ||
## Parameter table 33
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 34
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 35
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 36
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 37
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 38
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 39
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 40
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 41
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 42
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 43
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 44
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 45
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 1 | 60 | 12 ||
| 2 | 1 | 5 | 30 | 10 ||
| 3 | 1 | 0 | 100 | 17 ||
| 4 | 1 | 6 | 20 | 10 ||
| 5 | 1 | 30 | 90 | 50 ||
## Parameter table 46
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 1 | 60 | 12 ||
| 2 | 1 | 5 | 30 | 10 ||
| 3 | 1 | 0 | 100 | 17 ||
| 4 | 1 | 6 | 20 | 10 ||
| 5 | 1 | 30 | 90 | 50 ||
## Parameter table 47
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 2 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 48
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 49
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 50
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 51
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 1 | 60 | 12 ||
| 2 | 1 | 5 | 30 | 10 ||
| 3 | 1 | 0 | 100 | 17 ||
| 4 | 1 | 6 | 20 | 10 ||
| 5 | 1 | 30 | 90 | 50 ||
## Parameter table 52
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 2 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 53
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 54
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 55
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 56
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 1 | 60 | 12 ||
| 2 | 1 | 5 | 30 | 10 ||
| 3 | 1 | 0 | 100 | 17 ||
| 4 | 1 | 6 | 20 | 10 ||
| 5 | 1 | 30 | 90 | 50 ||
## Parameter table 57
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 2 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 58
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 59
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 60
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 61
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | -1 ||
| 1 | 1 | 1 | 60 | 12 ||
| 2 | 1 | 5 | 30 | 10 ||
| 3 | 1 | 0 | 100 | 17 ||
| 4 | 1 | 6 | 20 | 10 ||
| 5 | 1 | 30 | 90 | 50 ||
## Parameter table 62
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 2 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 63
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 64
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 65
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
## Parameter table 66
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 67
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
## Parameter table 68
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
## Parameter table 69
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
## Parameter table 70
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Programming unit type |
| 1 | 1 | Programming unit version major |
| 2 | 1 | Programming unit ersion minor |
## Parameter table 71
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 1 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 1 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
## Parameter table 72
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | -1 | 0 | 0 | DHW program: -1 own program, 0 - as HC |
| 1 | 1 | -1 | 0 | 0 | Circulation program: -1 own program, 0 - as HC |
| 2 | 1 | 0 | 2 | 2 | DHW operation mode |
| 3 | 1 | 0 | 2 | 2 | Circulation operation mode |
| 4 | 1 | -1 | 0 | 0 | DHW disinfection enabled |
| 5 | 1 | 0 | 7 | 1 | DHW disinfection weekday|
| 6 | 1 | 0 | 23 | 1 | DHW disinfection hour|
| 7 | 1 | -1 | 0 | 0 ||
| 8 | 1 | 60 | 80 | 60 | DHW maximum temperature |
| 9 | 1 | -1 | 0 | -1 | DHW single charge enabled |
## Parameter table 73
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Current date / year |
| 1 | 1 | Current date / month |
| 2 | 1 | Current time / hour |
| 3 | 1 | Current date / day |
| 4 | 1 | Current time / minute |
| 5 | 1 | Current time / second |
| 6 | 1 | Current date / weekday |
| 7 | 1 | Flags:<br/>bit 0 - summer time<br/>bit 5 - date not set<br/>bit 6 - time not set |
## Parameter table 74
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 2 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
## Parameter table 75
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
## Parameter table 76
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 1 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 1 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
| 27 | 1 ||
| 28 | 1 ||
| 29 | 1 ||
| 30 | 1 ||
| 31 | 1 ||
| 32 | 1 ||
| 33 | 1 ||
| 34 | 1 ||
| 35 | 1 ||
| 36 | 1 ||
| 37 | 1 ||
| 38 | 1 ||
| 39 | 1 ||
| 40 | 1 ||
| 41 | 1 ||
| 42 | 1 ||
| 43 | 1 ||
| 44 | 1 ||
| 45 | 1 ||
| 46 | 1 ||
| 47 | 1 ||
## Parameter table 77
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 1 ||
| 16 | 1 ||
| 17 | 1 ||
| 18 | 1 ||
| 19 | 1 ||
| 20 | 1 ||
| 21 | 1 ||
| 22 | 1 ||
| 23 | 1 ||
| 24 | 1 ||
| 25 | 1 ||
| 26 | 1 ||
| 27 | 1 ||
| 28 | 1 ||
| 29 | 1 ||
| 30 | 1 ||
| 31 | 1 ||
| 32 | 1 ||
| 33 | 1 ||
| 34 | 1 ||
| 35 | 1 ||
| 36 | 1 ||
| 37 | 1 ||
| 38 | 1 ||
| 39 | 1 ||
| 40 | 1 ||
| 41 | 1 ||
| 42 | 1 ||
| 43 | 1 ||
| 44 | 1 ||
| 45 | 1 ||
| 46 | 1 ||
| 47 | 1 ||
## Parameter table 78, 83, 88, 93, 98
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 5 | 1 | Heating type:<br/>1 - radiatior<br/>2 - convector<br/>3 - floor<br/>4 - room flow |
| 1 | 1 | 10 | 58 | 34 | Room temperature day |
| 2 | 1 | 12 | 60 | 42 | Room temperature night |
| 3 | 1 | 10 | 60 | 34 | Room temperature holiday |
| 4 | 1 | 0 | 10 | 0 | Maximum room influence |
| 5 | 1 | 0 | 99 | 40 | Room influence factor |
| 6 | 1 | -10 | 10 | 0 | Room temperature offset |
| 7 | 1 | 0 | 2 | 2 | Operating mode:<br/>0 - night<br/>1 - day<br/>2 - auto |
| 8 | 1 | -1 | 0 | 0 | Drying cycle active |
| 9 | 1 | 1 | 10 | 5 | Drying cycle temperature decrease |
| 10 | 1 | 1 | 40 | 5 | Drying cycle temperature increase |
| 11 | 1 | 25 | 60 | 45 | Drying cycle maximum flow temperature |
| 12 | 1 | 0 | 5 | 1 | Drying cycle reduced flow temperature duration |
| 13 | 1 | 1 | 5 | 1 | Drying cycle duration |
| 14 | 1 | 0 | 20 | 4 | Drying cycle maximum flow temperature duration |
| 15 | 1 | 30 | 90 | 75 | Maximum flow temperature (radiator) |
| 16 | 1 | 5 | 70 | 5 | Minimum flow temperature |
| 17 | 1 | 30 | 90 | 75 | Standard temperature (radiator) |
| 18 | 1 | 0 | 2 | 1 |  |
| 19 | 1 | -1 | 0 | 0 | Switch optimizations enabled |
| 20 | 1 | 10 | 60 | 60 | Parameter for switch off optimization (maximum ahead time) |
| 21 | 1 | -1 | 0 | -1 | DHW priority active |
| 22 | 1 | 9 | 31 | 17 | Summer operation temperature |
| 23 | 1 | -20 | 10 | 5 | Frost protection temperature |
| 24 | 1 | 0 | 20 | 5 | Boiler increase |
| 25 | 1 | 0 | 3 | 3 | Reduction mode:<br/>0 - shutdown<br/>1 - reduced operation<br/>2 - room setback<br/>3 - outdoor setback |
| 26 | 1 | 0 | 2 | 2 | Assigned operating unit:<br/>0 - none<br/>1 - RC2x<br/>2 - RC35 |
| 27 | 1 | 0 | 7 | 0 ||
| 28 | 1 | 0 | 2 | 1 | Frost protection temperature source:<br/>0 - disabled<br/>1 - outside temperature<br/>2 - room temperature |
| 29 | 1 | 5 | 80 | 40 | Parameter for targets calculation in room temperature control mode |
| 30 | 1 | 5 | 100 | 25 | Parameter for targets calculation in room temperature control mode |
| 31 | 1 | 0 | 100 | 10 | Parameter for targets calculation in room temperature control mode (rate of room temperature change ratio) |
| 32 | 1 | 1 | 3 | 1 | Heating system type:<br/>1 - radiator<br/>2 - convector<br/>3 - floor |
| 33 | 1 | 0 | 1 | 0 | Control mode:<br/>0 - outside temperature<br/>1 - room temperature |
| 34 | 1 | -1 | 0 | -1 | Heating circuit active |
| 35 | 1 | 25 | 60 | 50 | Maximum flow temperature (floor) |
| 36 | 1 | 25 | 60 | 45 | Standard temperature (floor) |
| 37 | 1 | 0 | 60 | 0 | Room temperature until next switch point |
| 38 | 1 | -31 | 10 | -31 | Outside temperature for reduce interruption |
| 39 | 1 | -20 | 10 | 5 | Outside temperature for reduce operation |
| 40 | 1 | -20 | 10 | 5 | Outside temperature for holiday operation |
| 41 | 1 | 0 | 3 | 2 | Holiday reduction mode |
## Parameter table 79, 84, 89, 94, 99
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Flags:<br/>bit 0 - switch off optimization active<br/>bit 1 - switch on optimization active<br/>bit 2 - auto mode<br/>bit 3 - DHW priority<br/>bit 4 - drying cycle active<br/>bit 5 - holiday operation<br/>bit 6 - frost protection active<br/>bit 7 - manual mode |
| 1 | 1 | Flags:<br/>bit 0 - summer operation<br/>bit 1 - daytime operation<br/>bit 4 - room temperature until next switch point override<br/>bit 5 - switch on optimization boost<br/>bit 7 - party operation |
| 2 | 1 | Room temperature target |
| 3 | 2 | Room temperature actual |
| 4 | 1 | Switch on optimization elapsed time |
| 5 | 1 | Switch off optimization elapsed time |
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 2 | Rate of room temperature change |
| 10 | 1 | Requested power of the boiler |
| 11 | 1 | Switching program state |
| 12 | 1 | Calculated target flow temperature |
| 13 | 1 | Flags:</br>bit 0 - no room temperature input, but needed<br/>bit 1 - reduce interrupted<br/>bit 2 - heating disabled |
## Parameter table 80, 85, 90, 95, 100
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 | Drying cycle phase |
| 1 | 1 | Drying cycle hour |
| 2 | 1 | Drying cycle day |
| 3 | 1 | Drying cycle temperature |
| 4 | 1 ||
| 5 | 1 | Drying cycle progress |
| 6 | 2 | Switch off optimization - ahead ticks factor |
| 8 | 1 | Switch off optimization - elapsed time |
| 10 | 2 | Switch on optimization - attenuated outside temperature post-boost |
| 11 | 2 | Switch on optimization - room temperature post-boost |
| 13 | 2 | Switch on optimization - room temperature pre-boost |
| 15 | 1 | Switch on optimization - elapsed time |
| 16 | 1 | Drying cycle backup - DHW system installed |
| 17 | 1 | Drying cycle backup - Anti-commute time |
| 18 | 1 | Drying cycle backup - Switch off hysteresis |
| 19 | 1 | Drying cycle backup - Switch on hysteresis |
## Parameter table 81, 86, 91, 96, 101, 103, 104
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 84 | * | * | * | Switching points:<br/>up to 42 points, 16bit values encoded as<br/>WWW--SSSTTTTTTTT<br/>W - weekday (0-6 - Mo-Su, 7 - unused)<br/>S - state (0 - off/night, 1 - on/day, 2-7 - unused)<br/>T - time (hour * 6 + minute / 10)<br/>* E790 - end of the program/unused point |
| 84 | 1 | 0 | 10 | 1 | Preset |
| 85 | 1 | 0 | 99 | 0 | Pause hours left |
| 86 | 1 | 0 | 99 | 0 | Party hours left |
| 87 | 1 | 1 | 31 | 1 | Holiday away start date - day |
| 88 | 1 | 1 | 12 | 1 | Holiday away start date - month |
| 89 | 1 | 0 | 99 | 0 | Holiday away start date - year |
| 90 | 1 | 1 | 31 | 1 | Holiday away end date - day |
| 91 | 1 | 1 | 12 | 1 | Holiday away end date - month |
| 92 | 1 | 0 | 99 | 0 | Holiday away end date - year |
| 93 | 1 | 1 | 31 | 1 | Holiday at home start date - day |
| 94 | 1 | 1 | 12 | 1 | Holiday at home start date - month |
| 95 | 1 | 0 | 99 | 0 | Holiday at home start date - year |
| 96 | 1 | 1 | 31 | 1 | Holiday at home end date - day |
| 97 | 1 | 1 | 12 | 1 | Holiday at home end date - month |
| 98 | 1 | 0 | 99 | 0 | Holiday at home end date - year |
## Parameter table 82, 87, 92, 97, 102
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 84 | * | * | * | Switching points:<br/>up to 42 points, 16bit values encoded as<br/>WWW--SSSTTTTTTTT<br/>W - weekday (0-6 - Mo-Su, 7 - unused)<br/>S - state (0 - off/night, 1 - on/day, 2-7 - unused)<br/>T - time (hour * 6 + minute / 10)<br/>* E790 - end of the program/unused point |
## Parameter table 105
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 0 | 0 ||
| 1 | 1 | 0 | 0 | 0 ||
| 2 | 1 | -50 | 50 | 0 ||
| 3 | 1 | 0 | 0 | 0 ||
| 4 | 1 | -1 | 0 | -1 ||
| 5 | 1 | -30 | 0 | -10 ||
| 6 | 1 | 0 | 2 | 1 ||
| 7 | 1 | 0 | 99 | 6 ||
| 8 | 1 | 0 | 99 | 0 ||
| 9 | 1 | 0 | 3 | 1 ||
| 10 | 1 | 0 | 0 | 0 ||
| 11 | 1 | -30 | 30 | 0 ||
| 12 | 1 | -30 | 30 | 0 ||
| 13 | 1 | -1 | 0 | 0 ||
| 14 | 1 | -1 | 0 | -1 ||
| 15 | 1 | 0 | 3 | 0 ||
| 16 | 1 | -8 | 13 | 0 ||
| 17 | 1 | 4 | 7 | 5 ||
| 18 | 1 | 15 | 50 | 28 ||
| 19 | 1 | 4 | 7 | 5 ||
| 20 | 1 | 15 | 50 | 40 ||
| 21 | 1 | -1 | 0 | -1 ||
| 22 | 1 | 0 | 4 | 0 ||
| 23 | 1 | 0 | 99 | 99 ||
| 24 | 1 | -1 | 0 | 0 ||
| 25 | 1 | 0 | 0 | 0 ||
| 26 | 1 | 0 | 0 | 0 ||
| 27 | 1 | 0 | 0 | 0 ||
## Parameter table 106
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 2 ||
| 4 | 2 ||
| 5 | 2 ||
| 6 | 2 ||
| 7 | 2 ||
## Parameter table 107
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
| 9 | 1 ||
| 10 | 1 ||
| 11 | 1 ||
| 12 | 1 ||
| 13 | 1 ||
| 14 | 1 ||
| 15 | 4 ||
| 16 | 1 ||
## Parameter table 108
| Index | Size | Description |
|-------|------|-------------|
| 0 | 2 ||
| 1 | 1 ||
| 2 | 2 ||
| 3 | 2 ||
| 4 | 1 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 4 ||
| 9 | 4 ||
## Parameter table 109
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 1 ||
| 4 | 1 ||
| 5 | 1 ||
## Parameter table 110
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 1 | 4 | 1 ||
| 1 | 1 | 10 | 58 | 34 ||
| 2 | 1 | 12 | 60 | 42 ||
| 3 | 1 | 0 | 2 | 2 ||
| 4 | 1 | 30 | 90 | 75 ||
| 5 | 1 | 5 | 70 | 5 ||
| 6 | 1 | 0 | 2 | 1 ||
| 7 | 1 | -1 | 0 | -1 ||
| 8 | 1 | 5 | 80 | 40 ||
| 9 | 1 | 5 | 100 | 25 ||
| 10 | 1 | 0 | 100 | 10 ||
| 11 | 1 | 1 | 8 | 1 ||
| 12 | 1 | -1 | 0 | 0 ||
| 13 | 1 | 0 | 60 | 0 ||
| 14 | 1 | -40 | 0 | -10 ||
| 15 | 1 | 0 | 60 | 18 ||
| 16 | 1 | 30 | 90 | 90 ||
| 17 | 1 | 9 | 31 | 17 ||
| 18 | 1 | 0 | 10 | 0 ||
| 19 | 1 | 0 | 99 | 40 ||
| 20 | 1 | -20 | 10 | 5 ||
| 21 | 1 | -20 | 10 | 5 ||
| 22 | 1 | -10 | 10 | 0 ||
## Parameter table 111
| Index | Size | Description |
|-------|------|-------------|
| 0 | 1 ||
| 1 | 1 ||
| 2 | 1 ||
| 3 | 2 ||
| 4 | 2 ||
| 5 | 1 ||
| 6 | 1 ||
| 7 | 1 ||
| 8 | 1 ||
## Parameter table 112
| Index | Size | Min | Max | Default | Description |
|-------|------|-----|-----|---------|-------------|
| 0 | 1 | 0 | 255 | 32 ||
| 1 | 1 | 0 | 255 | 32 ||
| 2 | 1 | 0 | 255 | 32 ||
| 3 | 1 | 0 | 255 | 32 ||
| 4 | 1 | 0 | 255 | 32 ||
| 5 | 1 | 0 | 255 | 32 ||
| 6 | 1 | 0 | 255 | 32 ||
| 7 | 1 | 0 | 255 | 32 ||
| 8 | 1 | 0 | 255 | 32 ||
| 9 | 1 | 0 | 255 | 32 ||
| 10 | 1 | 0 | 255 | 32 ||
| 11 | 1 | 0 | 255 | 32 ||
| 12 | 1 | 0 | 255 | 32 ||
| 13 | 1 | 0 | 255 | 32 ||
| 14 | 1 | 0 | 255 | 32 ||
| 15 | 1 | 0 | 255 | 32 ||
| 16 | 1 | 0 | 255 | 32 ||
| 17 | 1 | 0 | 255 | 32 ||
| 18 | 1 | 0 | 255 | 32 ||
| 19 | 1 | 0 | 255 | 32 ||
| 20 | 1 | 0 | 255 | 32 ||
| 21 | 1 | 0 | 255 | 32 ||
| 22 | 1 | 0 | 255 | 32 ||
| 23 | 1 | 0 | 255 | 32 ||
| 24 | 1 | 0 | 255 | 32 ||
| 25 | 1 | 0 | 255 | 32 ||
| 26 | 1 | 0 | 255 | 32 ||
| 27 | 1 | 0 | 255 | 32 ||
| 28 | 1 | 0 | 255 | 32 ||
| 29 | 1 | 0 | 255 | 32 ||
| 30 | 1 | 0 | 255 | 32 ||
| 31 | 1 | 0 | 255 | 32 ||
| 32 | 1 | 0 | 255 | 32 ||
| 33 | 1 | 0 | 255 | 32 ||
| 34 | 1 | 0 | 255 | 32 ||
| 35 | 1 | 0 | 255 | 32 ||
| 36 | 1 | 0 | 255 | 32 ||
| 37 | 1 | 0 | 255 | 32 ||
| 38 | 1 | 0 | 255 | 32 ||
| 39 | 1 | 0 | 255 | 32 ||
| 40 | 1 | 0 | 255 | 32 ||
| 41 | 1 | 0 | 255 | 32 ||
