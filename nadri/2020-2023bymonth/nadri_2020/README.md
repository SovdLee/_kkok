
## 파일 전부 합쳐서 data로 불러오는 코드
```python
import pandas as pd

url_template = "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_{month:02d}.csv"

dfs = []

# 1월부터 12월까지 가져오기
for month in range(1, 13):
    url = url_template.format(month=month)
    df = pd.read_csv(url)
    dfs.append(df)

data = pd.concat(dfs, ignore_index=True)

display(data.head())

```

---


## 월별 파일 raw 주소
```python
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_{month}.csv
```
