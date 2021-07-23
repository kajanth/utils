# utils

Based on Alpine. Includes curl, dig, nc, jq and fish for now.


```bash
docker run -ti ghcr.io/kajanth/utils:main sh
```

```bash
kubectl run -it utils --rm --image=ghcr.io/kajanth/utils:main sh
```

Run to get your public ip
```
myip="$(dig +short myip.opendns.com @resolver1.opendns.com)"
echo "My WAN/Public IP address: ${myip}"
```
