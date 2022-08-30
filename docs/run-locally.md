# Run local - Mamp,Xamp,Wamp
You can run the project in your local computer by using  Mamp,Xamp or Wamp
{% embed url="https://www.loom.com/share/35a324760fbc427b9978fcccea6cc525" caption="" %}

# Run local - Docker way

In Laravel 8, there is a new package available called [https://laravel.com/docs/8.x/sail](https://laravel.com/docs/8.x/sail).

We use this to run the site locally and test it.

### Step 1 - Install Docker

All you need is to install [https://www.docker.com/](https://www.docker.com/) on your computer.

After that extract the code and open it in the Terminal / Command prompt 

```text
cd poslion
./vendor/bin/sail up
```

The first time you run this can take some time 



### Step 2 - Install via CMD

After sail is running, open a new terminal window and navigate to the project.

execute

```text
sail artisan migrate --fresh --seed
```

This will set up \( seed \) the database.

Then execute / run

```text
cd storage
touch installed
```

This should create an empty file in **storage** folder, to let the system know that the project is installed. Then open the site on [localhost](http://127.0.0.1). 

You should see the site now

Login with the default credentials

**Username**: admin@example.com

**Password**: secret

