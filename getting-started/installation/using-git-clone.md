---
description: You need to have installed git in your server.
---

# Using Git Clone



{% hint style="info" %}
`master` branch is being considered as a stable, but not yet released to the public.
{% endhint %}

{% hint style="warning" %}
Installed the system under  `var/www` directory with a proper permissions.
{% endhint %}

1. from your terminal you can run:

<pre class="language-bash"><code class="lang-bash"><strong>$ git clone https://github.com/OSSAdmiral/Recruit.git
</strong></code></pre>

2. You need install the dependency package via composer and NPM:

{% code fullWidth="false" %}
```bash
$ composer install --optimize-autoloader --no-dev
$ npm install && npm run build
```
{% endcode %}

3. Create symbolic link from your public/storage

```bash
$ php artisan storage:link
```

4. You need to run caching to optimize system server response time

```bash
$ php artisan config:cache
```

5. Setup file and folder permissions

```bash
$ sudo chown -R www-data:www-data /var/www/Recruit
$ sudo chmod -R 775 /var/www/Recruit/app/storage
$ sudo chmod -R 775 /var/www/Recruit/app/bootstrap/cache
```

{% hint style="success" %}
:confetti\_ball: Congratulation! you've now completely installed system dependencies. Proceed to the next steps.
{% endhint %}
