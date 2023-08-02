# Memo Linux
## Set a date, time
```bash
date +%T -s "10:13:13"
```
## Find something in a gz file
```bash
find . -name "dpkg*.gz" -exec zgrep 'upgrade gitlab' \{\} \; 2>/dev/null
```

## Size of a folder
```bash
du -sh <folder_name>
```

## Git delete all tags names by `release-6`

```bash
git tag -l | grep release-6 | xargs -I % sh -c 'git tag -d %; git push --delete origin %'
```

Reverse ` -v`
