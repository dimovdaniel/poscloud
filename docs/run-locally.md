# Run local

In Laravel 8, there is new package available called [https://laravel.com/docs/8.x/sail](https://laravel.com/docs/8.x/sail).

We use this to run the site locally, and test it.

All you need is to install [https://www.docker.com/](https://www.docker.com/) in your compute.

After that, open the code and execute the command

```text
./vendor/bin/sail up
```

You can add alias for the sail command.

Then open the site on localhost, and the install window should appear.

One thing we needed to change in our .env was

\`\`\`text DB\_HOST=mysql

\`\`\`text

DB\_HOST=mysql

