# Getting Started
<div id="start" data-magellan-destination="start"></div>


Dive into creating your responsive email.

***

## The Boilerplate

Starting a new Ink project is fairly straightforward. If you aren&#8217;t using one of our [templates](templates), grab the boilerplate code from below to use as a starting point. While you can reference `ink.css` using a <kbd>&lt;link&gt;</kbd> tag for testing purposes, be sure to remove the <kbd>&lt;link rel="stylesheet" href="ink.css" /&gt;</kbd> statement and paste your CSS into the <kbd>&lt;style&gt;</kbd> tag in the head before running your email through an inliner.

###### Boilerplate.html

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="width=device-width"/>

    <link rel="stylesheet" href="wink.css"> <!-- For testing only -->

    <style type="text/css">

      /* Ink styles go here in production */

    </style>
    <style type="text/css">

      /* Your custom styles go here */

    </style>
  </head>
  <body>
    <table class="body">
      <tr>
        <td class="center" align="center" valign="top">
          <center>

          <!-- Email Content -->

          </center>
        </td>
      </tr>
    </table>
  </body>
</html>
```

If you&#8217;re applying a background color to your entire email, be sure to attach it to the table with a class of `body` as well as to the actual <kbd>&lt;body&gt;</kbd> tag, since some clients remove this by default.

###### Inline Styles

```html
<html>
...
<body style="background:#ddd">
  <table class="body" style="background:#ddd"> <!-- Background goes here too -->
    ...
  </table>
</body>
</html>
```

###### CSS

```css
body, .body {
  background: #ddd;
}
```

***

## Sending Your Email

Sending HTML email is a lot different than sending plain text email. While it may be tempting to just open the email in a browser and click &#8220;share&#8221; or to use the &#8220;Insert HTML&#8221; function of your favorite email client, this often strips off a lot of the styling and makes your email completely unusable on mobile devices.

To get the best results, we recommend that you send your HTML email using an [Email Service Provider (ESP)](http://en.wikipedia.org/wiki/Email_service_provider_(marketing)) such as [Mailchimp](http://mailchimp.com) or [Campaign Monitor](http://campaignmonitor.com). If you&#8217;re just running a quick test and don't want to sign up for an ESP, sending from the command line using a scripting language like [PHP](http://php.net/manual/en/function.mail.php) or [Ruby](http://ruby-doc.org/stdlib-2.0/libdoc/net/smtp/rdoc/Net/SMTP.html) usually works fine.

***

## Testing and Troubleshooting

Since targeting a [diverse range of email clients](#compatibility) requires some specific and rather quirky markup, Ink doesn&#8217;t always preview properly in the browser. When doing browser tests, we recommend using the latest version of [Chrome](http://google.com/chrome), [Safari](http://www.apple.com/safari/) or [Opera](http://www.opera.com/), since Ink doesn&#8217;t always display properly in Firefox or Internet Explorer.

Testing in the browser isn't enough, however, and you should always test in actual email clients. If you don't have access to the actual clients you want to test, a testing service like [Litmus](https://litmus.com/) or [Email on Acid](http://www.emailonacid.com/) can help.

If you're having trouble with an email, the first thing to check is the markup. Often times a simple error like a forgotten <kbd>&lt;tr&gt;</kbd> or a nested tag that&#8217;s been closed in the wrong order can wreak havoc on your design. If that&#8217;s not the problem, it could be an issue with your ESP. **Some senders prepend an <kbd>&lt;html&gt;</kbd> tag to your message, which causes the DOCTYPE tag to not be interpreted by the email recipient.** To see if this is what&#8217;s happening, try sending a test email to yourself and using the &#8220;show original&#8221; or &#8220;raw source&#8221; option in your mail client to manually inspect the code.
