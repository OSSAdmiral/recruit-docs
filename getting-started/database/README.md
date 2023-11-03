# Database



{% hint style="warning" %}
In this documentation, you're environment variable for the database should already been setup. If not yet then follow the instruction below.
{% endhint %}

1. Create a table on your preferred database

> For MySQL example: run the command below inside your mysql terminal.\
> $ CREATE DATABASE recruit

2. update your database credential in your `.env` file

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=recruit
DB_USERNAME=root
DB_PASSWORD=root
```

{% hint style="success" %}
:tada: Congratulations!, the system is now connect to the DB you have been setup.
{% endhint %}
