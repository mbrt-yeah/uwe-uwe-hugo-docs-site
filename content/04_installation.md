---
weight: 4
title: "Installation"
draft: false
---

## Installation

Independently of the installation methods described below you have to specify in the configuration file of your website-project that you want to built your site using the Uwe Uwe (u²) theme.

{{< tabs id="code-block-tabbed-01" >}}

  {{< tab title="JSON" >}}
  
   ```JSON
   {
       baseURL: "<Base Url of your website>",
       languageCode: "<Language of your website >",
       title: "<Title of your website >",
       theme: "uwe-uwe",

       ...
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   baseURL: "<Base Url of your website>"
   languageCode: "<Language of your website >"
   title: "<Title of your website >"
   theme: "uwe-uwe"

   ...
   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   baseURL = "<Base Url of your website>"
   languageCode = "<Language of your website >"
   title = "<Title of your website >"
   theme = "uwe-uwe"

   ...
   ```

  {{< /tab >}}

{{< /tabs >}}

### Manual download

You can download [the latest version of the Uwe Uwe (u²) theme](https://github.com/mbrt-yeah/uwe-uwe-hugo/releases) directly to the `/themes` directory of your website-project.

### Git submodule

You can add the Uwe Uwe (u²) theme as a git submodule by cloning it directly to the `/themes` directory of your website project using the following command:

```cmd
git submodule add https://github.com/mbrt-yeah/uwe-uwe-hugo.git themes/uwe-uwe
```
