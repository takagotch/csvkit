### csvkit
---
https://github.com/wireservice/csvkit

```
mkdir csvkit_tutorial
cd csvkit_tutorial

curl -L -O https://raw.githubusercontent.com/wireservice/csvkit/master/examples/realdata/ne_1033_data.xlsx
in2csv ne_1033_data.xlsx
in2csv ne_1033_data.xlsx > data.csv

cat data.csv
csvlook data.csv
csvlook data.csv | less -S
csvcut -n data.csv
csvcut -c 2,5,6 data.csv
csvcut -c country,item_name,quantity data.csv
csvcut -c county,item_name,quantity data.csv | csvlook | head
in2csv ne_1033_data.xlsx | csvcut -c country,item_name, quantity | csvlook | head
```

```
```

```
```

