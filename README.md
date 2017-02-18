# sky-dns delegated

## Configuration

I have linked to the skydns configuration section of their README in the docker compose file.

## Starting

```bash
docker-compose up -d etcd && sleep 3 && docker-compose up etcd skydns
```

## After

```bash
dig @localhost -p 10053 something.that.NAMESERVERS.resolves
```