# Goolge Cloud Shell (gcloud) Cheat Sheet

## Compute Instance

**Create instances**
```shell
gcloud compute instatnces create [instance name] \
--zone [cn-zone-#] \                                                           # (optional)
--machine-type [machine-type] \                                                # (optional)
--network-interface network=[network-name],subnet=[subnet-name]                # (optional)
```


**Delete instances**
```shell
gcloud compute instances delete [instance name] --zone [cn-zone-#]
```

**List all instance types**
```shell
gcloud compute machine-types list | cut -d' ' -f1 | sort | uniq
```
***Reference:*** [https://cloud.google.com/sdk/gcloud/reference/compute/instances/create](https://cloud.google.com/sdk/gcloud/reference/compute/instances/create)

---

**Firewall Rules Create**
```shell
gcloud compute firewall-rules create [firewall-rule-name] \
--network [network-name] \
--source-ranges [x.x.x.x/x] \
--rules tcp:[port],icmp] \
--action [allow|deny]
```
***Reference:*** [https://cloud.google.com/sdk/gcloud/reference/compute/firewall-rules/create](https://cloud.google.com/sdk/gcloud/reference/compute/firewall-rules/create)

---

