---
title: The Reference template
tableOfContents: false
---

<style>
.sl-container:where(.astro-7nkwcw3z) {
    max-width: none;
}
</style>

```````md
---
title: title
category: reference
owner: your email
created: YYYY-MM-DD
---

{Summarize what this reference article is about. Explain what all the entries defined on the page have in common.}

{It can be helpful to split up your reference page into subsets of related enries. For example, the reference page for an API endpoint might include subsets of entries for "General Requirements", "Request Parameters", and "Responses". The formats of entries might be different for each subset; for example, "General Requirements" might be a bulleted list, while "Request Parameters" and "Responses" are tables.}

## {subset of reference entries}

{table or other structured presentation of entries}

## Parameters

|Name |Type |Required |Description |
|:--- |:--- |:--- |:--- |
|productCode|`string`|Yes|Code of the document product to return the schema for. <br> <ul><li>Here is a bulleted list with a \| (pipe) inside a table.</li><li>Another bulleted list.<ul><li>An indented list</li></ul></li><li>Back to the list.</li></ul> |
|||||


```````