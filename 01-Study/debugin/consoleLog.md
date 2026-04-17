---
id: consoleLog
aliases: []
tags: []
---

# understanding console.log

To display data that is beeing feched to the front end use 'console.log'
EXAMPLE: console.log("FULL DATA:", data);

example of code

```lua
// call backend api
try {
    const data = await $fetch("https://localhost:8000/api/weather", {
      query: {
        location: location.value,
      },
    });

    console.log("FULL DATA:", data);
    console.log("DAYS:", (data as any).days);
    console.log((data as any).days[0]);
```

data is beeing feched and put in to the variable 'data'
we console.log 'data'

2. then we go to
