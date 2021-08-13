---
weight: 5
title: "Hugo Configuration"
draft: false
---

## Hugo Configuration

The recommended Hugo configuration when you are using the Uwe Uwe (u²) theme.

### Disable creation of contents

In order not to clutter the build-result with unnecessary files you can disable the creation of section, taxonomy, term and RSS contents using the [disableKinds](https://gohugo.io/getting-started/configuration/#disablekinds) option in your project configuration file.

{{< tabs id="code-block-tabbed-12" >}}

  {{< tab title="JSON" >}}
   ```Javascript
   {
       disableKinds: ["section", "taxonomy", "term", "RSS"]
   }
   ```
  {{< /tab >}}

  {{< tab title="Yaml" >}}
   ```YAML
   disableKinds:
      - "section"
      - "taxonomy"
      - "term"
      - "RSS"
   ```
  {{< /tab >}}

  {{< tab title="Toml" >}}
   ```TOML
   disableKinds = ["section", "taxonomy", "term", "RSS"]
   ```
  {{< /tab >}}

{{< /tabs >}}

### Markup related configurations

For markdown in notifications and sidenotes to be correctly displayed you have to set the 
`markup.goldmark.renderer.unsafe` flag to `true`.

{{< tabs id="code-block-tabbed-13" >}}

  {{< tab title="JSON" >}}
   ```Javascript
   {
       markup: {
           goldmark: {
               renderer: {
                   unsafe: true
               }
           }
       }
   }
   ```
  {{< /tab >}}

  {{< tab title="Yaml" >}}
   ```YAML
   markup:
      goldmark:
          renderer:
              unsafe: true
   ```
  {{< /tab >}}

  {{< tab title="Toml" >}}
   ```TOML
   [markup]
       [markup.goldmark]
           [markup.goldmark.renderer]
               unsafe = true
   ```
  {{< /tab >}}

{{< /tabs >}}

Furthermore, it has been found that the `igor` style of [Hugo's internal syntax highlighter](https://gohugo.io/content-management/syntax-highlighting/) works best with the design of the Uwe Uwe (u²) theme.

{{< tabs id="code-block-tabbed-14" >}}

  {{< tab title="JSON" >}}
   ```Javascript
   {
       markup: {
           goldmark: {
               highlight: {
                   style: "igor"
               }
           }
       }
   }
   ```
  {{< /tab >}}

  {{< tab title="Yaml" >}}
   ```YAML
   markup:
      goldmark:
          highlight:
              style: igor
   ```
  {{< /tab >}}

  {{< tab title="Toml" >}}
   ```TOML
   [markup]
       [markup.goldmark]
           [markup.goldmark.highlight]
               style = "igor"
   ```
  {{< /tab >}}

{{< /tabs >}}







