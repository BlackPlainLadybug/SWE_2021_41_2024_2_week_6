# SWE_2021_41_2024_2_week_6

## Week 4 Assignment

- [Happy number] (https://github.com/BlackPlainLadybug/SWE_2021_41_2024_2_week_4/blob/main/2022315193_%EC%B5%9C%EC%9C%A0%EC%84%9D.ipynb.ipynb)
```python
def isHappy(n):
  ns=[n]
  while True:
    n2=0
    for i in range(len(str(n))):
      n2+=int(str(n)[i])**2
    if n2==1:
      return  True
    if n2 in ns:
      return False
    ns.append(n2)
    n=n2
```
- Keep all n2s that derived by summing its digits' squares in ns until n2 is already in ns or n2 is 1.
- If there are loop return false, else return true.
---
## Week 5 Assignment

> ```bash docker exec <your container> cat /etc/os-release ```
> - print /etc/or-release dir of Docker container. It contain information about OS.

> ```bash docker exec <your container> git --version ```
> - Checking the version of git on Docker container

> ```bash docker exec <your container> python3 --version ```
> - Checking the version of git on Python container

> ```bash docker inspect --format="{{ .HostConfig.Binds }}" <container_name> ```
> - Print sharing file between container and host system in format
