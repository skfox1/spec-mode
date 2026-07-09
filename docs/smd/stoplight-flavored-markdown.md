# Stoplight Flavored Markdown Compatibility

This page intentionally includes Stoplight-style Markdown patterns that may not have direct equivalents.

{% callout type="warning" %}
This Stoplight callout should be checked after import.
{% /callout %}

{% tabs %}
{% tab label="JavaScript" %}
```js
fetch('https://api.example.com/users')
```
{% /tab %}
{% tab label="cURL" %}
```bash
curl https://api.example.com/users
```
{% /tab %}
{% /tabs %}

![Sized image](../../assets/images/overview.png "width=240")

Expected outcome: the page imports, but these components require manual visual review and likely rewriting.
