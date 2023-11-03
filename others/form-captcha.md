# Form Captcha



{% hint style="danger" %}
By default, the form is using a development captcha which is always return solved. This need to be updated by supplying the key.
{% endhint %}



### New Sites

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/?to=/:account/turnstile) and select your account.
2. Go to **Turnstile**.
3. Select **Add a site** and fill out the form.
4. Copy your sitekey and secret key.
5. update your `.env` file for the `TURNSTILE_SITE_KEY` and `TURNSTILE_SECRET_KEY`&#x20;

```
TURNSTILE_SITE_KEY=3x00000000000000000000FF
TURNSTILE_SECRET_KEY=1x0000000000000000000000000000000AA
```

### Existing sites

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/?to=/:account/turnstile) and select your account.
2. Go to **Turnstile**.
3. In the widget overview, select **Settings**.
4. Copy your sitekey and secret key.
5. update your `.env` file for the `TURNSTILE_SITE_KEY` and `TURNSTILE_SECRET_KEY`&#x20;

```
TURNSTILE_SITE_KEY=3x00000000000000000000FF
TURNSTILE_SECRET_KEY=1x0000000000000000000000000000000AA
```



***

{% hint style="info" %}
If you want to use Google ReCaptcha, follow the instruction below
{% endhint %}

1. Update the default captcha value by update the `captcha_provider_name` to `Google` .
   1. go to `Config` folder
   2. find `recruit.php` file and update the `captcha_provider_name` .
