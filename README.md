# InboxPager

An E-mail client for the Android (java) platform. Supports IMAP, POP, and SMTP protocols through SSL/TLS.

# Usage

In order to use this application, you have to enable SSL/TLS application-email-checking through your email account's web interface. Some email servers may have this feature already turned on (NOT GMAIL!, see below). If your account's server does not support this feature, this app won't work.

You can set up an account in InboxPager by going to "Settings" > "Add Account". There you have to enter your account's credentials and server parameters. If you don't know what your email account's server parameters are, use the automatic tools provided to find out, or enter and test your own configuration. Optionally, if you'd like to receive a sound or vibration notification, tick those settings. If you wish to have a specific account refresh only when you want it to, untick the "Allow in all-accounts-refresh" in that account's settings.

By default InboxPager DOES <b>NOT</b> KEEP "FULL MESSAGE" copies of emails. It just downloads the main textual contents of the message. If you wish to change this policy, you can do this in the settings for an individual account. Keeping full messages can consume your device's internal memory very quickly. In order to save emails, the full message must first be downloaded into the internal database. Also, unless the full email message is already inside the internal database, downloading attachments will require access to the internet.

# Features

The app can:

- Animate a smooth transition between visual contexts.

- Automatically convert texts from their declared character encoding to UTF-8. 

- Download your full email messages (with attachments inside).

- Download an individual attachment.

- Display server certificates used in the last connection.

- Keep track of your unread messages.

- Notify with sound of new messages (per user choice).

- Notify with device vibration of new messages (per user choice).

- Work with OpenPGP messages.

- Verify hostnames (if self-signed certificates aren't available).

# Permissions

InboxPager uses android permissions on the local device for the following reasons:

ACCESS_NETWORK_STATE, INTERNET:

Communication with user defined message servers. Downloading/Uploading messages.

VIBRATE:

Device can be made to vibrate, if new messages have arrived. Users can disable this setting from inside the application.

WRITE_EXTERNAL_STORAGE:

In order to save messages, or attachments, to the device.

READ_EXTERNAL_STORAGE:

In order to send messages with attachments.

## Requirements

In general - a network connection that does not implement (small) download quotas.

For a POP (Post Office Protocol 3) mail server:

- Support for the extensions "TOP", "SASL", and "UIDL".

- LOTS of internal phone memory.

