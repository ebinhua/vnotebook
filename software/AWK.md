# AWK


 -F 分隔符
$0 表示所有列
$1 第一列
``` bash
awk -F ','  '{print $1}' data1.csv 
awk 'BEGIN{FS=OFS=","}{print $1}' data1.csv 
```

类似vlookup的命令
```bash
awk 'BEGIN{FS=OFS=","}NR==FNR{w[$4]=$5","$6}NR>FNR{for(a in w) ... 
if(a==$4){print $1,$2,$3,$4,w[a]}}' data1.csv data2.csv
```

awk for 
``` bash
awk '{for(i=1;i<=NF;i++){print $i}}'
```

查找字符窜在第几列
```bash
awk -F ',' '{for(i=1;i<NF;i++)if($i==5){print i}}' data4.csv

awk -F ',' '{for(i=1;i<NF;i++)if($i~/匹配字符窜/){print i}}' data1.csv 
```
输出匹配字符串的行
awk ‘/字符串/’ file

NR and FNR:
https://www.linuxidc.com/Linux/2012-05/61174.htm