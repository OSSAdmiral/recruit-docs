---
description: Installation of sendmail in the server droplet / machine
---

# Server Sendmail

{% hint style="warning" %}
This guide is focus more on Linux OS
{% endhint %}

1. Firstly, install Sendmail using the command:

```
$ sudo apt-get install sendmail
```

2. Now configure /etc/hosts file. To find the hostname, use the command:

```
$ hostname
```

3. Then type the command:

```
$ sudo nano /etc/hosts
```

4. On the line starting with 127.0.0.1, add the hostname to the end so it looks the same as:

```
$ 127.0.0.1 localhost hostname
```

5. Now press Ctrl+x, then ‘Y’ to save and exit.
6. Run Sendmail’s config and answer ‘Y’ to everything

```
$ sudo sendmailconfig
```

7. Now restart Apache with the command:

```
$ sudo service apache2 restart
```

{% hint style="success" %}
:tada:Congrats!, your server can now send an email using our recruit application.
{% endhint %}



***

{% hint style="info" %}
Need to test if working fine?, follow steps below.
{% endhint %}

1. You can use the following instructions to send email using the sendmail command:

```bash
$ sendmail email_address < file.txt
```

> For example, I have created a file `file.txt` with the following text:
>
> ```
> Hello there !
> ```

2. The command for sending the message will be:

```
$ sendmail < file.txt james@example.com
```

<figure><img src="https://journaldev.nyc3.cdn.digitaloceanspaces.com/2019/02/sendmail-output.png" alt=""><figcaption></figcaption></figure>

> You can use -s option to specify the email subject.



***

> Reference: [https://www.digitalocean.com/community/tutorials/send-email-linux-command-line](https://www.digitalocean.com/community/tutorials/send-email-linux-command-line)
