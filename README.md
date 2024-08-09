# SMTP Configuration
## Gmail
* SMTP Server: smtp.gmail.com
* Port: 465
* Username: example@gmail.com
* Encryption: SSL
* Enable 2-Step Verification, create an App Password and use it in your SMTP setting.

In order to use Gmail email to send mail, you need to create an App Password.

1. Turn on 2-Step verification for your Gmail account
Enable 2-Step Verification in "Manage Your Google Account -> Security"

![image](https://user-images.githubusercontent.com/40499291/82523366-c1882900-9b4b-11ea-8b92-1862405286de.png)

2. Create an App Password
Create an App Password in "Manage Your Google Account -> Security" ([instruction](https://support.google.com/accounts/answer/185833?hl=en)).

Now you can use this App Password as a Password for Sending email.

## G Suite
* SMTP Server: smtp.gmail.com
* Port: 465
* Username: example@gmail.com
* Encryption: SSL
* Enable 2-Step Verification, create an App Password and use it in your SMTP setting.

In order to use G Suite email, you need to create an App Password for the G Suite user.

According to G Suite support App Passwords will work forever - this authentication method will not be deprecated in the future.

### 1. Allow G Suite users to turn on 2-step verification
As admin go to G Suite  [Security --> Basic Settings](https://admin.google.com/bsds.org/AdminHome?hl=en#SecuritySettings:flyout=basic)  and tick the  `Allow users to turn on 2-step verification`  checkbox:

![2020-05-21_10-01-33](https://user-images.githubusercontent.com/40499291/82522810-3f4b3500-9b4a-11ea-9a91-5c499402ada2.png)

### 2. Turn on 2-Step verification for a G Suite user
Follow  [this instruction](https://support.google.com/accounts/answer/185839). You can use same phone number for different G Suite users.

![2020-05-21_10-12-58](https://user-images.githubusercontent.com/40499291/82523366-c1882900-9b4b-11ea-8b92-1862405286de.png)

### 3. Create an App Password for a G Suite user
Follow  [this instruction](https://support.google.com/accounts/answer/185833?hl=en).

![2020-05-21_10-20-45](https://user-images.githubusercontent.com/40499291/82523736-c9949880-9b4c-11ea-9def-0aa7a9fe240f.png)

Now you can use this App Password as a Password for Sending email.

## Microsoft 365 Exchange
* SMTP Server: smtp.office365.com
* Port: 587
* Encryption: TLS
* Emails in Microsoft Exchange are sent via SMTP oAuth.

Sending emails works via the same Microsoft Exchange app (you don't need to create two different Microsoft Exchange apps).
If you haven't been using SMTP, you may need to enable it using  [these Microsoft instructions](https://docs.microsoft.com/en-us/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission). You'll also have to set a password if using a shared mailbox, and you may have to disable security defaults in Azure or it will override SMTP settings.

If you are receiving `CN='your.server.com' did not match expected CN='smtp.office365.com'` error - see [this](https://smackdown.blogsblogsblogs.com/2021/08/28/peer-certificate-did-not-match-smtp-office365-com/).

## Yandex.Connect Mail
* SMTP Server: smtp.yandex.com
* Port: 465
* Username: example@domain.com
* Encryption: SSL

More info [here](https://yandex.com/support/mail/mail-clients.html)
