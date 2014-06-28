# Panels
<div id="panels" data-magellan-destination="panels"></div>

Quickly highlight important content.

***

Add a class of `panel` to a <kbd>&lt;td&gt;</kbd> in a `.columns` table in order to give it a default border and background color. Great for offsetting important content or for quickly prototyping a layout.

###### Panel Markup

```html
<table class="twelve columns">
  <tr>
    <td class="panel">

      Panel content

    </td>
    <td class="expander"></td>
  </tr>
</table>
```

###### Panel Example

<iframe id="if-panels" src="examples/panels.html"></iframe>

***

## Examples

#### Sidebar Panel

A common patten is to have a panel section serve as a sidebar to offset it from the primary content.

###### Sidebar Panel Markup

```html
<table class="row">
  <tr>
    <td class="wrapper">

      <table class="eight columns">
        <tr>
          <td>

            Main content

          </td>
          <td class="expander"></td>
        </tr>
      </table>

    </td>
    <td class="wrapper last">

      <table class="four columns">
        <tr>
          <td class="panel">

            Panel content

          </td>
          <td class="expander"></td>
        </tr>
      </table>

    </td>
  </tr>
</table>
```

###### Sidebar Panel

<iframe id="if-panelSidebar" src="examples/panel-sidebar.html"></iframe>

#### Panels With Sub-grids

Nesting a sub-grid under a panel is non-intuitive, since the sub-grid columns would normally be applied to the <kbd>&lt;td&gt;</kbd> elements directly under the `.columns` table. To get around this, give the <kbd>&lt;td&gt;</kbd> a class of `.panel` and a class of `.sub-grid`. You can then put a <kbd>&lt;table&gt;</kbd> inside the <kbd>&lt;td&gt;</kbd> and create the sub-columns using the <kbd>&lt;td&gt;</kbd> elements of the inner table, as shown below.

###### Panel Sub-Grid Markup

```html
<table class="twelve columns">
  <tr>
    <td class="panel sub-grid">

      <table>
        <tr>
          <td class="six sub-columns">

            Left Sub-Column

          </td>
          <td class="six sub-columns">

            Right Sub-Column

          </td>
        </tr>
      </table>

    </td>
    <td class="expander"></td>
  </tr>
</table>
```

###### Sub-Grid Panel

<iframe id="if-panelSubGrid" src="examples/panel-sub-grid.html"></iframe>

***

## Compatibility

<div class="compatibility-section">
  <div class="row">
    <div class="large-9 columns">

Panels work as expected in most major email clients.

    </div>
    <div class="large-3 columns">
      [Toggle Full Table](#)
    </div>
  </div>

  <div class="row">
    <div class="small-12 columns">
      <table>
        <thead>
          <tr>
            <th width="30%">Client</th>
            <th width="10%"><span>Supported</span></th>
            <th width="60%"><span>Notes</span></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Apple Mail (Desktop)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Apple Mail (iOS)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Outlook (2000, 2002, 2003)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Outlook (2007, 2010, 2013)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Outlook (2011)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Thunderbird</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Android</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Gmail (Desktop)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Gmail (Mobile, iOS, Android)</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Outlook 2011 for Mac</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>AOL Mail</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Hotmail</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
          <tr>
            <td>Outlook.com</td>
            <td><span class="check">&#10004;</span></td>
            <td></td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</div>
