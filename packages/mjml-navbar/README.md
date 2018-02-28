## mjml-navbar

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/1830348/15317906/d6cef510-1c23-11e6-83d7-31e4e4f8ba2a.png" width="800px" />
</p>

Displays a menu for navigation with an optional hamburger mode for mobile devices.

```xml
<mjml>
  <mj-body>
    <mj-section background-color="#ef6451">
      <mj-column>
        <mj-navbar base-url="https://mjml.io" hamburger="hamburger" ico-color="#ffffff">
            <mj-navbar-link href="/gettings-started-onboard" color="#ffffff">Getting started</mj-navbar-link>
            <mj-navbar-link href="/try-it-live" color="#ffffff">Try it live</mj-navbar-link>
            <mj-navbar-link href="/templates" color="#ffffff">Templates</mj-navbar-link>
            <mj-navbar-link href="/components" color="#ffffff">Components</mj-navbar-link>
        </mj-navbar>
      </mj-column>
    </mj-section>
  </mj-body>
</mjml>
```

<p align="center">
  <a target="_blank" href="https://mjml.io/try-it-live/components/navbar">
    <img width="100px" src="https://mjml.io/assets/img/svg/TRYITLIVE.svg" alt="try it live" />
  </a>
</p>

### mjml-navbar

Individual links of the menu should we wrapped inside mj-navbar.


Standard Desktop:

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/1830348/15317906/d6cef510-1c23-11e6-83d7-31e4e4f8ba2a.png" width="800px" />
</p>

Standard Mobile:

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/1830348/15317917/e514d0a4-1c23-11e6-8e5a-c23da9ac1d4e.png" width="318px" />
</p>

Mode hamburger enabled:

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/1830348/15317922/f01c5c24-1c23-11e6-9b0c-95b0602da260.gif" width="309px" />
</p>

<aside class="notice">
  The "hamburger" feature only work on mobile device with all iOS mail client, for others mail clients the render is performed on an normal way, the links are displayed inline and the hamburger is not visible.
</aside>

<aside class="notice">
  All the attributes prefixed with <code>ico-</code> help to customize the hamburger icon. They only work with the hamburger mode enabled.
</aside>

attribute                   | unit               | description                                                                                      | default value
----------------------------|--------------------|--------------------------------------------------------------------------------------------------|-----------------
base url                    | string             | base url for children components                                                                 | n/a
hamburger                   | string             | activate the hamburger navigation on mobile if the value is hamburger                            | n/a
align                       | string             | align content left/center/right                                                                  | center
ico-open                    | ASCII code decimal | char code for a custom open icon (hamburger mode required)                                       | 9776
ico-close                   | ASCII code decimal | char code for a custom close icon (hamburger mode required)                                      | 8855
ico-padding                 | px                 | hamburger icon padding, supports up to 4 parameters (hamburger mode required)                    | 10px
ico-padding-top             | px                 | hamburger icon top offset (hamburger mode required)                                              | 10px
ico-padding-right           | px                 | hamburger icon right offset (hamburger mode required)                                            | 10px
ico-padding-bottom          | px                 | hamburger icon bottom offset (hamburger mode required)                                           | 10px
ico-padding-left            | px                 | hamburger icon left offset (hamburger mode required)                                             | 10px
ico-align                   | string             | hamburger icon alignment, left/center/right (hamburger mode required)                            | center
ico-color                   | color format       | hamburger icon color (hamburger mode required)                                                   | #000000
ico-font-size               | px                 | hamburger icon size (hamburger mode required)                                                    | 30px
ico-font-family             | string             | hamburger icon font (only on hamburger mode)                                                     | Ubuntu, Helvetica, Arial, sans-serif
ico-text-transform          | string             | hamburger icon text transformation none/capitalize/uppercase/lowercase (hamburger mode required) | none
ico-text-decoration         | string             | hamburger icon text decoration none/underline/overline/line-through (hamburger mode required)    | none
ico-line-height             | px                 | hamburger icon line height (hamburger mode required)                                             | 30px


### mjml-navbar-link


This component should be used to display an individual link in the navbar.

<aside class="notice">
  The mj-navbar-link component must be used inside a mj-navbar component only.
</aside>

attribute        | unit          | description                           | default value
-----------------|---------------|---------------------------------------|------------------------------
color            | color         | text color                            | #000000
font-family      | string        | font                                  | Ubuntu, Helvetica, Arial, sans-serif
font-size        | px            | text size                             | 13px
font-style       | string        | normal/italic/oblique                 | n/a
font-weight      | number        | text thickness                        | n/a
line-height      | px            | space between the lines               | 22px
text-decoration  | string        | underline/overline/none               | n/a
text-transform   | string        | capitalize/uppercase/lowercase/none   | uppercase
padding          | px            | supports up to 4 parameters           | 10px 25px
padding-top      | px            | top offset                            | n/a
padding-bottom   | px            | bottom offset                         | n/a
padding-left     | px            | left offset                           | n/a
padding-right    | px            | right offset                          | n/a
rel              | string        | specify the rel attribute             | n/a