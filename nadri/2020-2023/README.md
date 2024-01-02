## 데이터프레임(df) 으로 파일 가져오는 코드! 
```python
import pandas as pd

def get_data_by_input():
    year = int(input("년도를 입력하세요: "))
    start_month = int(input("시작 월을 입력하세요: "))
    end_month = int(input("끝 월을 입력하세요: "))

    url_template = f"https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023/nadri_{year}/nadri_{year}_{{month:02d}}.csv"

    dfs = []

    for month in range(start_month, end_month + 1):
        url = url_template.format(month=month)
        df = pd.read_csv(url)
        dfs.append(df)

    data = pd.concat(dfs, ignore_index=True)
    return data

df = get_data_by_input()
display(df.head())

```

---


## 월별 파일 raw 주소
```python
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023/nadri_{year}/nadri_{year}_{month}.csv
```
