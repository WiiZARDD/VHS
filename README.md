<p align="center">
<img src="https://img.shields.io/github/languages/top/WiiZARDD/VHS?color=6d00c1&label-style=flat-square" </a>
<img src="https://img.shields.io/github/last-commit/WiiZARDD/VHS?color=6d00c1&label-style=flat-square" </a>
<img src="https://img.shields.io/github/downloads/WiiZARDD/VHS/total?color=6d00c1&labellabel=1.4.6 Downloads&style=flat-square" </a>
<img src="https://img.shields.io/github/stars/WiiZARDD/VHS?color=6d00c1&label=Stars&style=flat-square" </a>
<img src="https://img.shields.io/github/forks/WiiZARDD/VHS?color=6d00c1&label=Stars&style=flat-square" </a>
</p>

 
</p>
<p align="center">
<a href="https://github.com/WiiZARDD/VHS/releases/">Fast Download</a> ㅤ•ㅤ
<a href="https://discord.gg/8Hw4g9GxSK">Discord</a> ㅤ•ㅤ
<a href="https://www.youtube.com/">Showcase</a>
</p>
</p>
<p align="center">
<a href="https://www.python.org/ftp/python/3.10.5/python-3.10.5-amd64.exe">Python v3.10</a>ㅤㅤ 
<a href="https://www.python.org/ftp/python/3.9.0/python-3.9.0-amd64.exe">Python v3.9</a>
 
---
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/TZ5nybB.png" />
		</td>
	</tr>
	<tr>
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/l4hwEtb.png" />
		</td>
	</tr>
	<tr>


<p align="center"> 
  <kbd>
<img src="https://i.imgur.com/zANEo7u.png"></img>
  </kbd>
</p>

### Settings:
- [x] - **Windows 10 / 11**
- [x] - **Download Python:** [v3.10](https://www.python.org/ftp/python/3.10.5/python-3.10.5-amd64.exe) **or** [v3.9](https://www.python.org/ftp/python/3.9.0/python-3.9.0-amd64.exe)

- [x] - **100% Safe!**
- [x] - **Fequently Updating**
- [x] - **Might Have Some Bugs**
- [x] - **Python Provided**

> **WARNING:** If you paid for VHS, you were scammed.

> **DO NOT** Install VHS from another source or you could get **Hacked/Scammed.**

## Installation

#### Compiled Version
```sh-session
Download: https://github.com/WiiZARDD/VHS/releases
Extract File
Download the latest release (VHS-HUB.zip) and Extract The Executable
Launch Program and Enjoy!
```

---


### <a id="code-example"></a>💻〢Proxy Support Example:

```py
    def fetchProxies(url, custom_regex):
        global proxylist
        try:
            proxylist = requests.get(url, timeout=5).text
        except Exception:
            pass
        finally:
            proxylist = proxylist.replace('null', '')
        custom_regex = custom_regex.replace('%ip%', '([0-9]{1,3}\\.[0-9]{1,3}\\.[0-9]{1,3}\\.[0-9]{1,3})')
        custom_regex = custom_regex.replace('%port%', '([0-9]{1,5})')
        for proxy in re.findall(re.compile(custom_regex), proxylist):
            proxieslog.append(f"{proxy[0]}:{proxy[1]}")

    proxysources = [
        ["http://spys.me/proxy.txt","%ip%:%port% "],
        ["https://proxylist.icu/proxy/", "<td>%ip%:%port%</td><td>http<"],
        ["https://proxylist.icu/proxy/1", "<td>%ip%:%port%</td><td>http<"],
        ["https://proxylist.icu/proxy/2", "<td>%ip%:%port%</td><td>http<"],
        ["https://proxylist.icu/proxy/3", "<td>%ip%:%port%</td><td>http<"],
        ["https://proxylist.icu/proxy/4", "<td>%ip%:%port%</td><td>http<"],
        ["https://proxylist.icu/proxy/5", "<td>%ip%:%port%</td><td>http<"],
        ["http://www.httptunnel.ge/ProxyListForFree.aspx"," target=\"_new\">%ip%:%port%</a>"],
        ["https://www.us-proxy.org/", "<tr><td>%ip%<\\/td><td>%port%<\\/td><td>(.*?){2}<\\/td><td class='hm'>.*?<\\/td><td>.*?<\\/td><td class='hm'>.*?<\\/td><td class='hx'>(.*?)<\\/td><td class='hm'>.*?<\\/td><\\/tr>"],
        ["https://free-proxy-list.net/", "<tr><td>%ip%<\\/td><td>%port%<\\/td><td>(.*?){2}<\\/td><td class='hm'>.*?<\\/td><td>.*?<\\/td><td class='hm'>.*?<\\/td><td class='hx'>(.*?)<\\/td><td class='hm'>.*?<\\/td><\\/tr>"],
        ["https://www.sslproxies.org/", "<tr><td>%ip%<\\/td><td>%port%<\\/td><td>(.*?){2}<\\/td><td class='hm'>.*?<\\/td><td>.*?<\\/td><td class='hm'>.*?<\\/td><td class='hx'>(.*?)<\\/td><td class='hm'>.*?<\\/td><\\/tr>"],
        ["https://raw.githubusercontent.com/sunny9577/proxy-scraper/master/proxies.json", "\"ip\":\"%ip%\",\"port\":\"%port%\","],
        ["https://raw.githubusercontent.com/fate0/proxylist/master/proxy.list", '"host": "%ip%".*?"country": "(.*?){2}",.*?"port": %port%'],
        ["https://raw.githubusercontent.com/clarketm/proxy-list/master/proxy-list.txt", '%ip%:%port% (.*?){2}-.-S \\+'],
        ["https://raw.githubusercontent.com/opsxcq/proxy-list/master/list.txt", '%ip%", "type": "http", "port": %port%'],
        ["https://www.hide-my-ip.com/proxylist.shtml", '"i":"%ip%","p":"%port%",'],
        ["https://api.proxyscrape.com/?request=getproxies&proxytype=http&timeout=6000&country=all&ssl=yes&anonymity=all", "%ip%:%port%"],
        ["https://raw.githubusercontent.com/TheSpeedX/SOCKS-List/master/http.txt", "%ip%:%port%"],
        ["https://raw.githubusercontent.com/shiftytr/proxy-list/master/proxy.txt", "%ip%:%port%"],
        ["https://raw.githubusercontent.com/scidam/proxy-list/master/proxy.json", '"ip": "%ip%",\n.*?"port": "%port%",']
    ]
    threads = [] 
    for url in proxysources:
        t = threading.Thread(target=fetchProxies, args=(url[0], url[1]))
        threads.append(t)
        t.start()
    for t in threads:
        t.join()

    proxies = list(set(proxieslog))
    with open(temp, "w") as f:
        for proxy in proxies:
            for i in range(random.randint(7, 10)):
                f.write(f"{proxy}\n")
    execution_time = (time.time() - startTime)
```
### <a id="code-example"></a>💻〢Auto Download Modules:

```py
import os 
import threading

try:
    import EXAMPLE v1
except:
    os.system("pip install EXAMPLE v1")
    import EXAMPLE v1

try:
    import EXAMPLE v2
except:
    os.system("pip install EXAMPLE v2")
    import EXAMPLE v2
```

<h1 align="center">
  <a id="top"></a>🔮 Thanks For Using VHS! 🔮
</h1>

<p align="center"> 
  <kbd>
<img src="https://cdn.discordapp.com/attachments/1016863471738040460/1017146049820905532/standard.gif"></img>
  </kbd>
</p>
<h2 align="center">
VHS HUB
    
sets@riseup.net 
</h2>
