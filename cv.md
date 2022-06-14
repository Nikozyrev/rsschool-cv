# Nikita Kozyrev
## Financial Manager
### About me and my work
I'm a financial manager in the IT sphere. My main passion in work is building tables and charts that can represent the situation and dynamics of all business aspects.  And the main reward is the best decisions that management can take based on my work.

And what I like in the process the most is coding. So I decided to go forward and become a software developer. I chose Frontend (JavaScript) and I'm actively moving in this direction now. But also I learned Python previously and prepared some projects that I used in my work (see code examples below).

**********
### Skills and Proficiency:
- Excel, Google sheets
- HTML5, CSS3
- Python Basics
- JavaScript Basics
- Git, GitHub
- VS Code, PyCharm

**********
### Code example:
*Bitcoin* and *Ethereum* actual course parser (Python Script).

```
from urllib.request import Request, urlopen
from datetime import date
from bs4 import BeautifulSoup
import ssl

ctx = ssl.create_default_context()
ctx.check_hostname = False
ctx.verify_mode = ssl.CERT_NONE

url = "https://coinmarketcap.com/"

courses = dict()

req = Request(url)
req.add_header('user-agent', 'my-app/0.0.1')
fname = urlopen(req).read()
soup = BeautifulSoup(fname, "lxml")

bitcoin = soup.find("a", { "href" : "/currencies/bitcoin/markets/" })
ethereum = soup.find("a", { "href" : "/currencies/ethereum/markets/" })
#rub = soup.find("span", { "class" : "bl_rub_ex" })

courses["Bitcoin"] = bitcoin.text
courses["Ethereum"] = ethereum.text
#courses["RUB"] = float(rub.text)


for k, v in courses.items():
    print(k,v)
```

**********
### Courses:
- Coursera Advanced Excel (completed)
- Coursera Python Basics (completed)
- RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)

**********
### Languages:
- **Russian** - Native
- **English** - Intermediate/Upper-intermediate

**********
### Contact information:
**E-mail:** n.i.kozyrev@gmail.com

**Telegram:** @Snakerist

[GitHub](https://github.com/Nikozyrev)

[LinkedIn](https://www.linkedin.com/in/%D0%BD%D0%B8%D0%BA%D0%B8%D1%82%D0%B0-%D0%BA%D0%BE%D0%B7%D1%8B%D1%80%D0%B5%D0%B2-3b344a185/)
