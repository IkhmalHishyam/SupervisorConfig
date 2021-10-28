# SupervisorConfig

## Install supervisor 

```
sudo apt-get install supervisor
```

## Access supervisor conf through

```
cd /etc/supervisor
```

## Command to open .conf file

```
cat supervisord.conf
```

## Command to edit .conf file

```
sudo nano supervisord.conf
```

## Add Root Path under include section 

```
files = /etc/supervisor/conf.d/*.conf #Your Root Path - Refer to laravel-worker.conf#
```

## Run these command to update your config

```
sudo supervisorctl reread
```

```
sudo supervisorctl update
```

## Start your supervisor

```
sudo supervisorctl start laravel-worker:*
```

## You can check whether your supervisor is running or not

```
sudo service supervisorctl status
```

Credit : CraigGoesCoding

