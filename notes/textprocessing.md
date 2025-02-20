1. [grep](#grep)
2. [sed](#sed)
3. [awk](#awk)
4. [cut](#cut)
5. [tr](#tr)
6. [column](#column)
7. [Cases](#cases)
* [Line count](#line-count)

## grep

Parallel log grep:
```bash
ls /var/log/HOSTS/*/*.service.{a,b,c,d}.ru/archive/service.log-20241003*.gz 2>/dev/null | \
xargs -P 20 -I {} grep search_string {} > results.log
```

## sed
```bash
# remove lines containing 'DEBUG'
sed '/DEBUG/d' service.log

# the same and update service.log with sed output (GNU)
sed -i '/DEBUG/d' service.log

# the same for BSD sed
sed -i '' '/DEBUG/d' service.log

```

## awk

## cut

## tr

## column
```bash
(printf "PERM LINKS OWNER GROUP SIZE DAY MONTH YEAR NAME\n"; ls -l | sed 1d) | column -t
```

## Cases

### Line count
```bash
grep -c . file.txt
grep -c ^ file.txt
awk 'END{print NR}' file.txt

# wc counts only New line characters, thus result may differ from grep and awk
wc -l file.txt
```