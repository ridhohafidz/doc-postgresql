# How to Uninstall PostgreSQL #

```bash
sudo apt-get --purge remove postgresql
```

In case that doesn't do the trick, try listing all PostgreSQL related software and dependencies by executing this command:
```bash
dpkg -l | grep postgres
```


Uninstall packages listed by that command by executing:
```bash
sudo apt-get --purge remove postgresql-9.4 postgresql-client-9.4 postgresql-client-common postgresql-common postgresql-contrib-9.4
```
![Purge all PostgreSQL dependencies](../images/purge_all_psql.png)
