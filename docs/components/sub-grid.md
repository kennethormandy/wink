# Sub-Grid
<div id="sub-grid" data-magellan-destination="sub-grid"></div>

A non-stacking grid for even more versatile layouts.

***

#### Grids Within Grids

While the Ink grid can’t be nested like its [Foundation counterpart](http://foundation.zurb.com/docs/components/grid.html), Ink does provide a nestable sub-grid for when one grid just isn't enough. By applying a `.sub-columns` class (as well as a numbered class, same as the primary grid) to a <kbd>&lt;td&gt;</kbd> tag underneath a `.columns` table, you can sub-divide the `.columns` table into sub-columns.

The last `.sub-columns` <kbd>&lt;td&gt;</kbd> in the `.columns` <kbd>&lt;table&gt;</kbd> should be given a class of `last` in order for the gutter padding to be properly maintained.

###### Basic Sub-Grid Example

```html
<table class="row">
  <tr>
    <td class="wrapper">

      <table class="eight columns">
        <tr>
          <td class="eight sub-columns">

            .eight.sub-columns

          </td>
          <td class="four sub-columns last">

            .four.sub-columns

          </td>
          <td class="expander"></td>
        </tr>
      </table>

    </td>
    <td class="wrapper last">

      <table class="four columns">
        <tr>
          <td>

            .four columns

          </td>
          <td class="expander"></td>
        </tr>
      </table>

    </td>
  </tr>
</table>
```

###### Non-Collapsing Sub-Grid Columns

<iframe id="if-subGrid" src="examples/basic-sub-grid.html"></iframe>

***

## Compatibility

<div class="compatibility-section">
  <div class="row">
    <div class="large-9 columns">

The sub-grid works as expected in most major email clients.

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
