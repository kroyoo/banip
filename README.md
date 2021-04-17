# 记录爆破ssh黑名单IP

## 免责申明

如果你的IP不小心进入我的黑名单列表，造成误会，请发issue或者邮件联系我，请附上一定的证明，您并没有恶意爆破。否则，不会从我的列表删除，我会保留日志和对应的时间截图。


## 获取fail2ban-client IP
`fail2ban-client status sshd | grep 'Banned IP list' | sed 's/.*://' |  sed 's/ /\n/g' | sed 's/[ \t]*//g' `
