# Memo Linux
## Set a date, time
date +%T -s "10:13:13"
## Find something in a gz file
find . -name "dpkg*.gz" -exec zgrep 'upgrade gitlab' \{\} \; 2>/dev/null
