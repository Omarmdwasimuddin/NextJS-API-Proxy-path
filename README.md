## NextJS API---> Working With Proxy Path

### Define proxy which path execute
![](https://imgur.com/MRxg5fq.png)

```bash
import { NextRequest } from "next/server";
import { NextResponse } from "next/server";


export function proxy(request: Request){
    console.log("proxy is new name of middleware")
}

export const config = {
    matcher:['/api/:path*']
}
```
---
