# laravel trouble shootings
nginx php7.2 laravel ubuntu8.0.4 502error noVendorDir

# you should check it

- [ ] install composer without *apt-get* it is not current version and cannot self update
- [ ] install php newest version you can check in [laravel hompage](https://laravel.com/docs/5.7)
- [ ] check your path to where install the composer or laravel/installer the right path is *~/.config/composer/vendor/bin*


# Donot use composer create-project

```bash
composer global require laravel/installer #it's should be print install location
```
and you need append path to .bashrc

```bash
sudo nano ~/.bashrc
```

i was typed the like this. you must be check where laravel installed

```bash
export PATH=~/.config/composer/vendor/bin:$PATH
...
```

thanks

