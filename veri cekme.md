### R' a veri cekmek

---

■	oncelikle dosyanizi R'in calistigi klasore (working directory) tasiyin.

■	dosyaniz excel dosyasi ile .csv uzantili olarak kaydedin.

■	.txt ya da .csv dosyasini acarak inceleyin. 

---

Dikkat etmeniz gereken seyler: 


■	ilk satir degisken isimleri icin ayrilmis mi,

■	Excel Turkce ise csv dosya kaydedilirken ayrac olarak ; kullanacaktir.

■	degiskenler birbirinden hangi ayrac (seperator = sep) ile ayrilmis ( , ; / tab)

■	ondalik basamagini belirlemek icin nokta ya da virgul mu kullanilmis (R ondalik basamagi icin nokta kullanir verinizde virgul kullanilmis ise degistirmelisiniz) 

■	verinin yapisini inceleyin, sadece sayilardan mi olusuyor, yoksa karakter (text) ya da alfenumerik (hem harf hem sayi) veriler var mi, eksik gozlem(missing data) var mi? varsa nasil ifade edilmis. ( ?, -, NA, . ya da bos olabilir) R eksik gozlem icin NA kullanir


```r
read.table()
```

```r
read.csv()
```

```r
read.txt()  #fonksiyonlari verinizi R'a cekecektir. 
```

```r
?read.csv #ile detayli kullanimini gorebilirsiniz)
 ```

```r
read.csv("benioku", header=T, sep=;) 
```

---

foreign paketini kullanarak bircok formattan R'a veri cekebilrsiniz

http://cran.r-project.org/web/packages/foreign/index.html

http://cran.r-project.org/web/packages/foreign/foreign.pdf,

```r
install.packages("foreign")

library(foreign)

read.spss("benioku.sav") # gibi...
```





---

http://www.wekaleamstudios.co.uk/posts/importing-data-into-r-from-text-files/#more-3

http://cran.r-project.org/doc/manuals/R-data.pdf

http://www.ats.ucla.edu/stat/r/faq/inputdata_R.htm

http://www.biostat.jhsph.edu/~bcaffo/statcomp/files/ingo.R.3.notes.pdf

https://science.nature.nps.gov/im/datamgmt/statistics/r/fundamentals/index.cfm




---

R'da olusturdugunuz veri setini ya da analizlerin sonuclarini farkli formatlara aktarmak isterseniz:

http://www.statmethods.net/input/exportingdata.html
