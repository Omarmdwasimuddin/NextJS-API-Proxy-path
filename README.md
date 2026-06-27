## NextJS API---> Working With Proxy Path

### Define proxy which path execute
##### home page not proxy executed.
![](https://imgur.com/MRxg5fq.png)
##### /api/:path* proxy executed.
![](https://imgur.com/yf7EJpo.png)

```bash
import { NextRequest, NextResponse } from "next/server";


export function proxy(request:NextRequest){
    console.log("proxy is new name of middleware")
}

export const config = {
    matcher:['/api/:path*']
}
```
---

### Include about page for proxy executed.
![](https://imgur.com/nQf2tlz.png)

```bash
import { NextRequest, NextResponse } from "next/server";


export function proxy(request:NextRequest){
    console.log("proxy is new name of middleware")
}

export const config = {
    matcher:['/api/:path*', '/about',]
}
```
---
