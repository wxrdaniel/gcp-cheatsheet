# Goolge Cloud Shell (gcloud) Cheat Sheet

## Compute Instance

**Create instances**
```shell
gcloud compute instatnces create [instance name] --zone [cn-zone-#] --machine-type [machine-type]
```

**Delete instances**
```shell
gcloud compute instances delete [instance name] --zone [cn-zone-#]
```

**List all instance types**
```shell
gcloud compute machine-types list | cut -d' ' -f1 | sort | uniq
```
