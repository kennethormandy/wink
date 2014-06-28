# Buttons
<div id="buttons" data-magellan-destination="buttons"></div>

Dynamic and effective calls to action.

***

## Structure

To create buttons that look great in most clients, make a table of class `button` to wrap your <kbd>&lt;a&gt;</kbd> tag. Buttons expand to the full width of their container by default, so if you don't want them to expand all the way, consider placing them in a [sub-grid](#sub-grid) or [block-grid](#block-grid) element.

###### A Basic Button

```html
<table class="button">
  <tr>
    <td>
      <a href="#">Button Label</a>
    </td>
  </tr>
</table>
```

***

## Style Classes

Several built in styling classes can be applied to the same element as the `button` class is applied to in order to adjust the button's appearance.

#### Size

Size classes affect the button's vertical padding. The available size classes are:

<table>
  <tr>
    <td>`.button` (same as `.small-button`)</td>
  </tr>
  <tr>
    <td>`.tiny-button`</td>
  </tr>
  <tr>
    <td>`.small-button`</td>
  </tr>
  <tr>
    <td>`.medium-button`</td>
  </tr>
  <tr>
    <td>`.large-button`</td>
  </tr>
</table>

#### Color

Color classes denote the purpose of the button, and are used to change its background color. The available color classes are:

<table>
  <tr>
    <td>none (same as `.primary`)</td>
  </tr>
  <tr>
    <td>`.primary`</td>
  </tr>
  <tr>
    <td>`.secondary`</td>
  </tr>
  <tr>
    <td>`.alert`</td>
  </tr>
  <tr>
    <td>`.success`</td>
  </tr>
</table>

#### Border Radius

Radius classes cause the corners of the buttons to be rounded in clients that support the <kbd>border-radius</kbd> property. The available radius classes are:

<table>
  <tr>
    <td>none (no border-radius)</td>
  </tr>
  <tr>
    <td>`.radius`</td>
  </tr>
  <tr>
    <td>`.round`</td>
  </tr>
</table>

***

## Examples

Buttons expand to the width of their parent container by default, so it's recommended that you contain them within a sub-grid or a relatively small number of columns on the main grid.

###### Button Demo

All the button modifiers demonstrated. The rows of buttons are contained to `.four.columns` or `.six.columns` sections of the grid for clarity.

<iframe id="if-buttons" src="examples/buttons.html"></iframe>

***

## Compatibility

<div class="compatibility-section">
  <div class="row">
    <div class="large-9 columns">

The buttons are compatible with most major clients.

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
