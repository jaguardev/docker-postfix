# Postfix installation based on Alpine


## Example

In this example:
* postfix configured as relay
* sasl auth enabled

Run:
```
docker-compose up
```

Send an e-mail with your favorite client using credentials:

Server: __localhost__

Port: __25__

Login: __donald@example.com__

Password: __melania__

Encryption: __None__

Authentication: __PLAIN__

## Notes

In this example ```sasldb2``` was pre-built, use ```saslpasswd2``` utility to customize:

```
saslpasswd2 -c -u example.com donald
```
