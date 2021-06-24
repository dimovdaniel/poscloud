# Run local

In Laravel 8, there is new package available called [https://laravel.com/docs/8.x/sail](https://laravel.com/docs/8.x/sail).

We use this to run the site locally, and test it.

All you need is to install [https://www.docker.com/](https://www.docker.com/) in your compute.

After that, open the code and execute the command

```text
./vendor/bin/sail up
```

One thing we needed to change in our .env was

\`\`\`text DB\_HOST=mysql

\`\`\`text

DB\_HOST=mysql

## Option 1: Install via web UI

Then open the site on [localhost](http://127.0.0.1), and the install window should appear.


## Option 2: Install via CMD

After you have setup the .env and sail is running, open new terminal - command line and navigate to the project. 

execute
```text
sail artisan migrate --fresh --seed
```

This will setup the database.

Then execute / run
```text
cd storage
touch installed
```
This should create empty file in storage, to let the system know that the project is installed.
Then open the site on [localhost](http://127.0.0.1).
You should see the site now


