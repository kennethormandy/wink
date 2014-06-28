# Visibility Classes
<div id="visibility-classes" data-magellan-destination="visibility-classes"></div>

Selectively show content for different screen sizes.

***

By adding a visibility class to an element, you can show or hide it based on screen size. Visibility classes can be used on any element. Due to Outlook's lack of support for certain CSS properties, the Ink visibiility classes should be used in conjunction with conditional comments to ensure that the content is properly hidden (or shown) in Outlook 2007/2010/2013.

Note: If you're using a visibility class on an image, be sure to apply it to the parent element, not to the image itself.

###### Using Visibility Classes

```html
<table class="row">
  <tr>
    <td class="wrapper last">

      <!--[if !mso]><!-- -->
        <table class="twelve columns show-for-small">
          <tr>
            <td class="panel">

              .show-for-small

            </td>
            <td class="expander"></td>
          </tr>
        </table>
      <!--<![endif]-->

      <table class="twelve columns hide-for-small">
        <tr>
          <td class="panel">

            .hide-for-small

          </td>
          <td class="expander"></td>
        </tr>
      </table>

    </td>
  </tr>
</table>
```

###### Content Visibility

<iframe id="if-visibilityClasses" src="examples/visibility-classes.html"></iframe>

***

## Breakdown

Available visibility classes:

<table>
  <tr>
    <td>`.hide-for-small`</td>
  </tr>
  <tr>
    <td>`.show-for-small`</td>
  </tr>
</table>

***

## Compatibility

<div class="compatibility-section">
  <div class="row">
    <div class="large-9 columns">

Visibility classes work as expected in most major email clients, but do not currently support **Gmail**.

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
            <td><span class="x">&#10008;</span></td>
            <td>Not yet implemented. Support will be added soon.</td>
          </tr>
          <tr>
            <td>Gmail (Mobile, iOS, Android)</td>
            <td><span class="x">&#10008;</span></td>
            <td>Not yet implemented. Support will be added soon.</td>
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
