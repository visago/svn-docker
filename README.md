# Simple SVN server via docker using SVN protocol

```
docker run -d --name=svn --restart=always -v /home/svn:/svn -p 3690:3690 visago/svn 
```

On host machine, "cd /home/svn", "svnadmin create repo-name", then edit /home/svn/repo-name/conf/* ! Disable anonymous !