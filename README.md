run

```
fluentd -c ./fluent/fluent.conf -vv   
```

send event

```
curl -i -X POST -d 'json={"action":"login","user":2}' http://localhost:8888/test.cycle
```


kill

```
pkill -f fluentd 
```
