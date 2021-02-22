# Postgresql & PgAdmin

# Requirements:
docker-compose

# Konfigurasi environment
change UID and GROUPS in .env file ,
how to check ID
```bash
echo "UID=$UID GROUPS=$GROUPS"
```

if your output : `UID= GROUPS=` null,
```bash
export UID=$(id -u)
export GROUPS=$(id -g)
```

how to edit `.env` via command line
```bash
sed -i "s/^UID=.*/UID=$UID/" .env
sed -i "s/^GROUPS=.*/GROUPS=$GROUPS/" .env

```
# Quick Start
```bash
docker-compose up -d
```

# Access To PgAdmin
```bash
http://localhost:3030
```
