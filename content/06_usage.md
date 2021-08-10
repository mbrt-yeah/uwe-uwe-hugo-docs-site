---
weight: 6
title: "Usage"
draft: true
---

## Usage

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

### Blockquote

> It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running 
> for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.
>
> -- <cite>Benjamin Franklin</cite>

### Code Inline

The function `selectAll()` highlights all the text in the input field so the user can, for example, copy or delete the text.

### Code Block Simple (No Syntax Higlighting)

```
const type = "Hello World";

const fn = test(type) { 
    return "blaa"; 
}

fn();
```

### Code Block Simple (Syntax Higlighting via Hugo)

```Javascript
const type = "Hello World";

const fn = test(type) { 
    return "blaa"; 
}

fn();
```

### Code Block Tabbed (No Syntax Higlighting)

{{< tabs id="code-block-tabbed-02" >}}

  {{< tab title="Typescript" >}}
  
   ```
   const type = "Hello World from tabpanel 01";

   const fn = test(type) {
     return "blaa"; 
   }

   fn();
   ```

  {{< /tab >}}

  {{< tab title="Javascript" >}}

   ```
   const type = "Hello World from tabpanel 02";

   const fn = test(type) {
     return "blaa"; 
   }

   fn();
   ```

  {{< /tab >}}

{{< /tabs >}}

### Code Block Tabbed (Syntax Higlighting via Hugo)

{{< tabs id="code-block-tabbed-03" >}}

  {{< tab title="Typescript" >}}
  
   ```Javascript
   const type = "Hello World from tabpanel 01";

   const fn = test(type) {
     return "blaa"; 
   }

   fn();
   ```

  {{< /tab >}}

  {{< tab title="Javascript" >}}

   ```Javascript
   const type = "Hello World from tabpanel 02";

   const fn = test(type) {
     return "blaa"; 
   }

   fn();
   ```

  {{< /tab >}}

{{< /tabs >}}

### Footnotes

#### Classical Hugo Footnote

Here is a simple footnote using the classical Hugo syntax[^a]. The footnote will be displayed at the end of this page.

[^a]: This is the simple footnote using the classical Hugo syntax

### Custom Shotcode Footnote

Here's a simple footnote using a custom shortcode{{< fn id="1" />}}. The footnote will be displayed as a sidenote.

{{% fn id="1" %}}
This is the simple footnote using the custom shortcode syntax #1
{{% /fn %}}

And here is another simple footnote using a custom shortcode{{< fn id="2" />}}. The footnote will be again be displayed as a sidenote.

{{% fn id="2" %}}
This is the simple footnote using the custom shortcode syntax #2
{{% /fn %}}

### List Ordered

1. List Item 1
2. List Item 2
   1. List Item 2.1
      1. List Item 2.1.1
      2. List Item 2.1.2
   2. List Item 2.2
   3. List Item 2.3
3. List Item 3

### List Unordered

- List Item 1
- List Item 2
  - List Item 2.1
    - List Item 2.1.1
    - List Item 2.1.2
  - List Item 2.2
  - List Item 2.3
- List Item 3

### Notifications

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

{{< notification type="info" title="Info" >}}
This is an information
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

{{< notification type="warning" title="Warning" >}}
This is a warning
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

{{< notification type="danger" title="Danger" >}}
This is a danger notification
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

### Notifications as Sidenotes

{{< notification type="info" title="Info" sidenote="right" >}}
This is an information
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

{{< notification type="warning" title="Warning" sidenote="right" >}}
This is a warning
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

{{< notification type="danger" title="Danger" sidenote="left" >}}
This is a danger notification
{{< /notification >}}

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

It works, ha ha ha ha, it works. I finally invent something that works. What the hell is this? George: you ever think of running for class president? Do you mind if we park for a while? Now, of course not, Biff, now, I wouldn't want that to happen.

### Table

|   #   | Surname  | Name     |
| :---: | :---     | :---     |
|   1   | Müller   | Matthias |
|   2   | Meier    | Mirko    |