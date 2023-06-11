## Manufacturing without creating BOM

**It is recommended to use BOM for Manufacturing for consistency and to avoid repetitive work.**

However, if you wish to perform it manually, the workaround is to create Stock Entries:

1) Create a **Stock Entry** with **Purpose** as **Material Transfer to Manufacture.**

![](https://docs.erpnext.com/files/EsxLtl4.png)

2) Create a **Stock Entry** with **Purpose** as **Manufacture, the Item which is being Manufactured will have a Target Warehouse and other Items(Raw Materials) will have a Source Warehouse.**

![](https://docs.erpnext.com/files/voUKccc.png)

﻿_Blue Dot: Item is being received._

_Orange Dot: Item is being issued._