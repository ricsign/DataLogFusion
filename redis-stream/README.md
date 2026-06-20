Set up from Redis cloud 

```bash
sudo apt install redis-tools
```

Connect to database using tool (also available to copy paste from redis dashboard):

```bash
redis-cli -u redis://default:<key>@<hostname>:<port>
```

```bash
# add a stream
XADD <stream_name> <ID> <field1> <value1> [field2 value2 ...]

e.g 

XADD /data/acc_x 123 x 5 y 10 z 15
```