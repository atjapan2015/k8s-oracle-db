
step1: modify database password

```
vi oracle-db-sts.yaml
```

change vaule of ORACLE_PWD to your desired thing

```
        - name: ORACLE_PWD
          value: TOdo__9090
```

step2: deply

```sh
kubectl apply -f .
```

```
ALTER SESSION SET container = pdb1;

GRANT
    DBA
TO pdbadmin;
```

DB Opeation Reference:
https://qiita.com/kawakawaryuryu/items/ae51bee866a57f178fe5
