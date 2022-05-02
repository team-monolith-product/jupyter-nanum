# jupyter-nanum
나눔 고딕 글꼴을 주피터에서 즉시 사용할 수 있도록 링크와 코드 예시를 제공합니다.

```
import matplotlib.pyplot as plt
from matplotlib import font_manager

with open('NanumGothic.ttf', 'wb') as f: 
    f.write(urllib.request.urlopen("https://github.com/team-monolith-product/jupyter-nanum/raw/main/NanumGothic.ttf").read())

font_path = 'NanumGothic.ttf'  # Your font path goes here
font_manager.fontManager.addfont(font_path)
prop = font_manager.FontProperties(fname=font_path)

plt.rcParams['font.family'] = prop.get_name()
```
