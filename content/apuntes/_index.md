+++
title = 'Apuntes'
date = 2023-09-19T11:54:20+02:00
draft = false
+++

# Markdown

Badge

{{% badge %}}Main{{% /badge %}}
{{% badge style="primary" title="Version" %}}Configuration{{% /badge %}}
{{% badge style="red" icon="angle-double-up" %}}Search{{% /badge %}}
{{% badge style="info" %}}New{{% /badge %}}
{{% badge color="fuchsia" icon="fab fa-hackerrank" %}}Galery{{% /badge %}}


Button

{{% button style="primary" icon="php" href="https://gohugo.io/" %}} Get Hugo {{% /button %}}


Children

{{% children sort="weight" %}}

{{ partial "shortcodes/children.html" (dict
  "page" .
  "sort" "weight"
)}}


OpenAPI

{{< openapi src="https://petstore3.openapi.io/api/v3/openapi.json" >}}


Expand

{{% expand title="Click to expand" %}} 
 Text
{{% /expand %}}


Highlight

{{< highlight lineNos="true" hl_lines="2 4"
 wrap="true" lineNoStart="1" type="php" >}}
# the hardest part is to start writing code; here's a kickstart; just copy and paste this; it's free; the next lines will cost you serious 
print("Hello")
print(" ")
print("World")
print("!")
{{< /highlight >}}


include

{{% include "shortcodes/datos.txt" %}} 
{{% include "shortcodes/INCLUDE_ME.md" %}}


Math

{{< math align="center" >}}
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$
{{< /math >}}


Mermaid

{{< mermaid >}}
---
title: Example Diagram
---
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{<strong>Decision</strong>}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}


Notice

{{< notice style="primary" title="Shortcode Noticieas" icon="skull-crossbones" >}}
Esto es una noticia importante
# esto es un titulo md  

<h1>Esto es un título de html</h1>
{{< /notice >}}

