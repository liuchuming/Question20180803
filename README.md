# Question
Q1:ubuntu 解决“无法获得锁 /var/lib/dpkg/lock -open （11：资源暂时不可用）”的方法
A1:强制解锁sudo rm /var/cache/apt/archives/lock
          sudo rm /var/lib/dpkg/loc
