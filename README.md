ContactForm
===========

How to install and use:

1.  Place the contactform folder in your craft/plugins folder.
2.  Go to Settings->Plugins from your Craft control panel and enable the Contact Form plugin.
3.  Click on “Contact Form” to go to the plugin’s settings page.
4.  Enter the email address you would like the contact requests to be sent to.

Your contact form template can look something like this:

    <form method="post" action="" accept-charset="UTF-8">
        <input type="hidden" name="action" value="contactform/sendMessage">

    <h3><label for="fromEmail">From Email</label></h3>
    <input id="fromEmail" type="text" name="fromEmail">

    <h3><label for="fromName">From Name</label></h3>
    <input id="fromName" type="text" name="fromName">

    <h3><label for="subject">Subject</label></h3>
    <input id="subject" type="text" name="subject">

    <h3><label for="message">Message</label></h3>
    <textarea rows="10" cols="40" id="message" name="message"></textarea>

    <input type="submit" value="Submit">
</form>

Note that "fromName" and "subject" are both optional fields.  The only required ones are "fromEmail" and "message".