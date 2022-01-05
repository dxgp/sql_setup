# Steps for installing SQL

## Step 1: Use Brew to get SQL
```shell
brew install mysql
```

Wait for it to complete.

## Step 2: Setup mySQL
Technically, mySQL is a server. Think of a server as a machine. To be able to connect to a machine, it must be turned on. Run the below command and brew will start the mySQL machine every time the laptop boots up:
```shell
brew services start mysql
```

By default, there's no password on mySQL. To set up SQL, run:
```
mysql_secure_installation
```

There will be a few questions:
1. Validate password component: Answer no. Then it will ask you if you for a new password. Enter whatever you want.
2. Remove anonymous users: Answer yes.
3. Disallow root login: Answer no.
4. Remove test database: Answer no.
5. Reload privelage tables: Answer yes.

Next, enter the password you want.

Now, to get the SQL prompt, enter the following in your terminal:

```shell
mysql -u root -p
```
Then, enter the password and you're in!
