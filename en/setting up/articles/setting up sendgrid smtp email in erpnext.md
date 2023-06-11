SMTP, or simple mail transfer protocol, is a quick and easy way to send email from one server to another. SendGrid provides an SMTP service that allows you to deliver your email via our server instead of your client or server. ERPNext comes built-in with a configured email client so that you can send and receive emails in ERPNext and append to documents if required.

**Integrating SendGrid's Web API**

SendGrid’s SMTP API allows developers to specify custom handling instructions for e-mail using an X-SMTPAPI header inserted into the message.

**Step 1:** You need to create an API key to authenticate your application. In this case, _ERPNext_. Learn more about integrating SendGrid with SMTP [here](https://sendgrid.com/docs/API_Reference/SMTP_API/integrating_with_the_smtp_api.html)

![](https://docs.erpnext.com/files/5Wqn0hV.png)

**Step 2:** Once your _API key_ has been created, you need to configure it in your ERPNext account > Create a **New** **Email Account.**

**Email Address:** _Your Email Address_

**Email Login ID:** _API Key_ \[API key generated in Step 1\]

**Password:** _Your Password_

**Service:** Select "_SendGrid_"

![](https://docs.erpnext.com/files/Q9to7Iu.png)

Now **save** this information and you have successfully configured the SendGrid SMTP Email in ERPNext.

Power to you!

\-----