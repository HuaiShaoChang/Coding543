# Coding543
Murmur or note from my coding life.

## Tips
### Linux(I'm using Debian.)
#### Newbie
- 查詢指令資訊：`type <command>`
<br />![](https://i.imgur.com/nZB4RAx.png)
- 查詢 shell 內建(builtin)指令：`help <command>`
<br />![](https://i.imgur.com/ko3E7wb.png)
- 查詢檔案類型：`file <filename>`
<br />![](https://i.imgur.com/q1EsUYR.png)
- man page 懶人包：`whatis <command>`
<br />![](https://i.imgur.com/2ckWctW.png)
#### Beginner
- 搜尋指令/檔案的 package：`dpkg-query --search <filename or fullpath>`, `dpkg-query -S <command>` for short.
<br />![](https://i.imgur.com/r8nKzhE.png)
#### Advanced
- I have no advanced skill. :pensive:
#### Expert
- I have no expert skill. :pensive:

## Murmurs
### 2019/01/06
- 遠端 Debian 主機上的 A 帳號可以用 key 登入，剛剛用 `ssh-copy-id` 把 public key 傳給 B 帳號後，ssh 還是一直跳輸入密碼。`cat /var/log/auth.log` 說我 `/home/B/.ssh` 的權限不對，才發現不知道幾百年前中邪，把 .ssh 的 group 改成 git，`chown B:B .ssh` 就好了XD
