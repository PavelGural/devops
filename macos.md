## Removal

### Cleanup disk

``` bash
# https://github.com/tw93/Mole
# detect changes
mo clean --dry-run
# run cleanup
mo clean

# docker cleanup
docker system prune --volumes --force
docker rmi $(docker images -q) -f

# check out storage
df -h # detect under /System/Volumes/Data
```

### Remove app

If you don't find an app in Applications folder, how to remove:

Go to the Apple Menu () > **System Settings** > **General** > **Storage**.
Click the **"i"** icon next to Applications.
Scroll through the list to find the **app**.
Select it and click **Delete**.

## Useful apps
- Blackmagic RAW Speed Test # From Dima
