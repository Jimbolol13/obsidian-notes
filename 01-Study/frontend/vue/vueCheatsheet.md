---
id: vueCheatsheet
aliases: []
tags: []
---

Here i write all my front end notes to remember

<strong></strong>
is beeing used to display text with a tronger bold look (so thicker text)

# using a ?

using a ? when caling specific data from youre back and is used in order to prevent a crash

Example:

```lua
      <p>
        <strong>Tomorrows temperature:</strong>
        {{ weather?.days?.[1]?.temp ?? "N/A" }} °C
      </p>
```
