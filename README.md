
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
grant create session,pdb_dba to pdbadmin;
```
