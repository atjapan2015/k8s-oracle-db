
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
    SYSOPER, DBA, PDB_DBA, RESOURCE, CONNECT,
    CREATE SESSION,
    CREATE PLUGGABLE DATABASE,
    CREATE TABLE,
    UNLIMITED TABLESPACE
TO pdbadmin;
```
