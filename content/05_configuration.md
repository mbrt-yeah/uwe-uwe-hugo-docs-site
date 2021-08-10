---
weight: 5
title: "Configuration"
draft: false
---

## Configuration

### Hugo-Specific Configuration Parameters

### Custom Configuration Parameters

All custom configuration parameters have to be set in the `params.uweuwe` section of the configuration file of your website-project.

{{< tabs id="code-block-tabbed-04" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       baseURL: "<Base Url of your website>",
       languageCode: "<Language of your website >",
       title: "<Title of your website >",
       theme: "uwe-uwe",

       ...

       params: {
           uweuwe: {
               ...
           }
       }
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

   params:
       uweuwe:
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

   [params]
       [params.uweuwe]
           ...
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Metadata

You can specify different information that serve as metadata for your website.

{{< tabs id="code-block-tabbed-05" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       params: {
           uweuwe: {
               metadata: {
                   author: "<WEBSITE_AUTHOR_NAME>"
               }
           }
       }
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   params:
       uweuwe:
           metadata:
               author: "<AUTHOR_NAME>"
   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   [params]
       [params.uweuwe]
           [params.uweuwe.metadata]
               authors = "<AUTHOR_NAME>"
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Logo

The logo is displayed at the top of the website.

If you don't want to display the logo just set the value of the `logo.display` parameter to `false`.

{{< tabs id="code-block-tabbed-06" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       params: {
           uweuwe: {
               logo: {
                   display: true,
                   src: "<PATH_TO_LOGO_FILE>"
               }
           }
       }
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   params:
       uweuwe:
           logo: 
               display: true # Possibile values: true | false
               src: "<PATH_TO_LOGO_FILE>"
   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   [params]
       [params.uweuwe]
           [params.uweuwe.logo]
               display = true # Possibile values: true | false
               src = "<PATH_TO_LOGO_FILE>"
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Short Description

The short description is displayed below the title of your website.

If you don't want to display the short description just set the value of the `shortDesc.display` parameter to `false`.

{{< tabs id="code-block-tabbed-07" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       params: {
           uweuwe: {
               shortDesc: {
                   display: true,
                   value: "<WEBSITE_SHORT_DESCRIPTION>"
               }
           }
       }
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   params:
       uweuwe:
           shortDesc: 
               display: true # Possibile values: true | false
               value: "<WEBSITE_SHORT_DESCRIPTION>"
   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   [params]
       [params.uweuwe]
           [params.uweuwe.shortDesc]
               display = true # Possibile values: true | false
               value = "<WEBSITE_SHORT_DESCRIPTION>"
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Platform Links

The platform links are displayed below the short description of the website.

You can choose between the following display modes:

- as-text: Displays a textual link to the specified platforms.
- as-icons: Displays only an iconized link to the specified platforms.
- as-icons-and-text: Displays an iconized link to the specified platforms with a text below.

If you don't want to display the platform links just set the value of the `platformLinks.display` parameter to `false`.

You can specify an unlimited number of platform links simply by adding entries to the `platformLinks.platforms` array/set. Every entry is composed of the following fields:

- name: Name of the platform
- display: Show or hide the platform link
- iconSrc: Path to the platform icon
- target: Target of the platform link
- text: Text of the platform link
- title: Title of the platformn link

{{< tabs id="code-block-tabbed-08" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       params: {
           uweuwe: {
               platformLinks: {
                   display: true,
                   displayMode: "as-icons-and-text" 

                   platforms: [
                       {
                           name: "<PLAFTORM_NAME>",
                           display: true,
                           iconSrc: "<PATH_TO_PLATFORM_ICON>",
                           target: "<LINK_TARGET>",
                           text: "<LINK_TEXT>",
                           title: "<LINK_TITLE>"
                       },

                       ...
                   ]
               }
           }
       }
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   params:
       uweuwe:
           platformLinks: 
               display: true # Possibile values: true | false
               displayMode: "as-icons-and-text" # Possible values: as-text | as-icons | as-icons-and-text

               platforms: 
               -   name: "PLAFTORM_NAME"
                   display: true # Possibile values: true | false
                   iconSrc: "<PATH_TO_PLATFORM_ICON>"
                   target: "<LINK_TARGET>"
                   text: "<LINK_TEXT>"
                   title: "<LINK_TITLE>"

               ...

   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   [params]
       [params.uweuwe]
           [params.uweuwe.platforms]
               display = true # Possibile values: true | false
               displayMode = "as-icons-and-text" # Possible values: as-text | as-icons | as-icons-and-text

               platforms = [
                   {
                       name = "<PLAFTORM_NAME>",
                       display = true, # Possibile values: true | false
                       iconSrc = "<PATH_TO_PLATFORM_ICON>",
                       target = "<LINK_TARGET>",
                       text = "<LINK_TEXT>",
                       title = "<LINK_TITLE>"
                   },

                   ...
               ]
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Table of Contents

{{< notification type="info">}}
The table of contents is created automatically based upon the <code>title</code> attribute in the front-matter of your content pages.
{{< /notification >}}

The table of contents is displayed below the platform links of your website.

If you don't want to display the table of contents just set the value of the `toc.display` parameter to `false`.

{{< tabs id="code-block-tabbed-09" >}}

  {{< tab title="JSON" >}}
  
   ```Javascript
   {
       params: {
           uweuwe: {
               toc: {
                   display: true
               }
           }
       }
   }
   ```

  {{< /tab >}}

  {{< tab title="Yaml" >}}

   ```YAML
   params:
       uweuwe:
           toc: 
               display: true # Possibile values: true | false
   ```

  {{< /tab >}}

  {{< tab title="Toml" >}}

   ```TOML
   [params]
       [params.uweuwe]
           [params.uweuwe.toc]
               display = true # Possibile values: true | false
   ```

  {{< /tab >}}

{{< /tabs >}}

#### Markdown Render Hooks

The Uwe Uwe (u²) theme uses [Markdown Render Hooks](https://gohugo.io/getting-started/configuration-markup/#markdown-render-hooks) to alter the HTML output of images, links and headings.
