
## 파일 전부 합쳐서 data로 불러오는 코드
```python
urls = [
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_01.csv?token=GHSAT0AAAAAACMFUPUUYZSK45OQ6FTKTOWKZMUBF6Q",
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_02.csv?token=GHSAT0AAAAAACMFUPUUNMZ6UFORMC3SO7IAZMUBGEQ",
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_03.csv?token=GHSAT0AAAAAACMFUPUVGIJDCPXLK2VQHMY4ZMUBGLQ"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_04.csv?token=GHSAT0AAAAAACMFUPUUFMN2MFPDIXEL5WLUZMUBHCA"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_05.csv?token=GHSAT0AAAAAACMFUPUVXFYT5BBB4IFNPJ2EZMUBHIA"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_06.csv?token=GHSAT0AAAAAACMFUPUUUNEJP23POTGB7JFAZMUBHPQ"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_07.csv?token=GHSAT0AAAAAACMFUPUVOHIJJWYIK45FFTDIZMUBHVA"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_08.csv?token=GHSAT0AAAAAACMFUPUUESPMURAVYWLLYNO6ZMUBH3A"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_09.csv?token=GHSAT0AAAAAACMFUPUU7GNGBBJPDHH2S23IZMUBH7Q"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_10.csv?token=GHSAT0AAAAAACMFUPUVOJJSHPO6HKPGWMK2ZMUBIDQ"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_11.csv?token=GHSAT0AAAAAACMFUPUULYX6GOQM5VXY7MY6ZMUBIMA"
    "https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_12.csv?token=GHSAT0AAAAAACMFUPUVZKHOJSK35E3BKE5CZMUBIQA"
]

dfs = []

for url in urls:
    df = pd.read_csv(url)
    dfs.append(df)

data = pd.concat(dfs, ignore_index=True)

display(data.head())
```

---


## 월별 파일 raw 주소

- 1월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_01.csv?token=GHSAT0AAAAAACMFUPUUYZSK45OQ6FTKTOWKZMUBF6Q
- 2월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_02.csv?token=GHSAT0AAAAAACMFUPUUNMZ6UFORMC3SO7IAZMUBGEQ
- 3월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_03.csv?token=GHSAT0AAAAAACMFUPUVGIJDCPXLK2VQHMY4ZMUBGLQ
- 4월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_04.csv?token=GHSAT0AAAAAACMFUPUUFMN2MFPDIXEL5WLUZMUBHCA
- 5월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_05.csv?token=GHSAT0AAAAAACMFUPUVXFYT5BBB4IFNPJ2EZMUBHIA
- 6월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_06.csv?token=GHSAT0AAAAAACMFUPUUUNEJP23POTGB7JFAZMUBHPQ
- 7월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_07.csv?token=GHSAT0AAAAAACMFUPUVOHIJJWYIK45FFTDIZMUBHVA
- 8월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_08.csv?token=GHSAT0AAAAAACMFUPUUESPMURAVYWLLYNO6ZMUBH3A
- 9월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_09.csv?token=GHSAT0AAAAAACMFUPUU7GNGBBJPDHH2S23IZMUBH7Q
- 10월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_10.csv?token=GHSAT0AAAAAACMFUPUVOJJSHPO6HKPGWMK2ZMUBIDQ
- 11월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_11.csv?token=GHSAT0AAAAAACMFUPUULYX6GOQM5VXY7MY6ZMUBIMA
- 12월
https://raw.githubusercontent.com/SovdLee/nadri_kkok/main/nadri/2020-2023bymonth/nadri_2020/nadri_2020_12.csv?token=GHSAT0AAAAAACMFUPUVZKHOJSK35E3BKE5CZMUBIQA
