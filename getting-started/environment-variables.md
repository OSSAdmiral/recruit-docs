# Environment Variables



{% hint style="warning" %}
Run _**php artisan generate:key**_ if you haven't done it yet.
{% endhint %}

1. Setup up your default mailer by changing this parameters from your `.env` file

```git
MAIL_MAILER=smtp
MAIL_HOST=mailpit
MAIL_PORT=1025
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null
MAIL_FROM_ADDRESS="hello@example.com"
MAIL_FROM_NAME="${APP_NAME}"
```

2. Disable debugging errors by changing `APP_DEBUG` from `True` to `False`

```
APP_DEBUG=true
```

3. Change your `APP_NAME` and `APP_URL` based on your current domains.
4. Change `APP_ENV` to `Production`&#x20;
5. Update your database connection credentials

```git
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

