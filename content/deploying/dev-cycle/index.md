---
title: "Development Cycle"
weight: 2
---

## OMG, this is SO easy...

Here is the developer workflow for maintaining your site.

{{<mermaid>}}
graph LR;
    A("fa:fa-code Visual Studio Code")== commit / push ===B("fa:fa-github GitHub");
    B== build / deploy ===C("fa:fa-globe-americas Live on the Internet");
    classDef d stroke-dasharray:5,5;
    classDef b stroke:#000,stroke-width:2px;
    classDef blue fill:#33a1ff; 
    classDef red fill:#ef2020;
    class A b
    class A d
    class A blue
    class B b
    class C red
    class C b
{{< /mermaid >}}

## Enjoy!

That's it, literally... from not having anything at all in place to now having a fully functioning blog site!
