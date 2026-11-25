# Cross-user rendering probe

This file is an inert security-test fixture. The markers below only set
page-local JavaScript variables if the dashboard renders untrusted content as
HTML. They do not transmit data.

<img src=x onerror=window.__mrx_body_img=1>

<svg onload=window.__mrx_body_svg=1></svg>

<details open ontoggle=window.__mrx_body_toggle=1>
  <summary>mrx details probe</summary>
  body marker
</details>

<iframe srcdoc="<script>parent.__mrx_body_iframe=1</script>"></iframe>

<a id="mrx-js-link" href="javascript:window.__mrx_body_js_link=1">mrx javascript link</a>

[markdown javascript link](javascript:window.__mrx_md_js_link=1)

![markdown image probe](x)

```html
<img src=x onerror=window.__mrx_code_img=1>
```
