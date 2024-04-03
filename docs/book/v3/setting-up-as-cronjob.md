# Setting up as cronjob

```text
*   *   *   *   *   /opt/plesk/php/7.4/bin/php /var/www/vhosts/example.com/httpdocs/bin/cli.php demo:command -q
```

or

```text
*   *   *   *   *   cd /var/www/vhosts/example.com/httpdocs/bin && /opt/plesk/php/7.4/bin/php ./cli.php demo:command -q
```

Adapt the command to your specifications by replacing **7.4** with your PHP version and **example.com** with your domain name.

Note the **-q** (or **--quiet**) option at the end of the command - it serves as a flag to inform the Application that no output should be returned (unless it's an error).
