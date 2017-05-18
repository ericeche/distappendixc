## Appendix C distribution run   5/15/2017

## Schema Wellpoint_54005New20170409 
	
		   
# epi_pacs and epi_provider_PACs tables.sql

```
mysql> use Wellpoint_54005New20170409;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> source epi_pacs and epi_provider_PACs tables.sql;
ERROR 1061 (42000): Duplicate key name 'emeid'
ERROR 1061 (42000): Duplicate key name 'asmed'
Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 17478 rows affected (0.59 sec)
Records: 17478  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 654248 rows affected (11.95 sec)
Records: 654248  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 666756 rows affected (11.54 sec)
Records: 666756  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.03 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 33 rows affected (2.68 sec)
Records: 33  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 672289 rows affected (12.38 sec)
Records: 672289  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 666756 rows affected (13.70 sec)
Records: 666756  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.03 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 717 rows affected (2.73 sec)
Records: 717  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 671606 rows affected (13.05 sec)
Records: 671606  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.01 sec)

Query OK, 666756 rows affected (15.06 sec)
Records: 666756  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.03 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 86950 rows affected (4.53 sec)
Records: 86950  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 585522 rows affected (12.11 sec)
Records: 585522  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.03 sec)

Query OK, 672472 rows affected (19.32 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 672472 rows affected (16.73 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.01 sec)

Query OK, 672472 rows affected (16.82 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 672472 rows affected (16.94 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 672472 rows affected (17.22 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.01 sec)

Query OK, 672472 rows affected (17.74 sec)
Records: 672472  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.03 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected (0.03 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 9746713 rows affected (3 min 6.72 sec)
Records: 9746713  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 9746713 rows affected (4 min 6.33 sec)
Records: 9746713  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 3208757 rows affected (10 min 20.35 sec)
Records: 3208757  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 3208757 rows affected (1 min 13.92 sec)
Records: 3208757  Duplicates: 0  Warnings: 0

Query OK, 741571 rows affected (47.10 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 101357 rows affected, 11990 warnings (11.22 sec)
Records: 101357  Duplicates: 0  Warnings: 11990


```		   
		   

# RA Input files.sql 

##    

```
mysql> source RA Input files.sql
Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 309216 rows affected (5.86 sec)
Records: 309216  Duplicates: 0  Warnings: 0

Query OK, 66754 rows affected (4.81 sec)

```
# PAC Rate RA program.R

```
ubuntu@Cert:/ecrfiles/git/prometheus_distribution/ecrfiles/post_ec/RSPR$Rscript PAC\ Rate\ RA\ program.R 

Attaching package: ‘dplyr’

The following objects are masked from ‘package:plyr’:

    arrange, count, desc, failwith, id, mutate, rename, summarise,
    summarize

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union

Loading required package: Matrix

Attaching package: ‘Matrix’

The following object is masked from ‘package:tidyr’:

    expand

Loading required package: foreach
Loaded glmnet 2.0-9

ResourceSelection 0.3-2 	 2017-02-28

Attaching package: ‘reshape’

The following object is masked from ‘package:Matrix’:

    expand

The following objects are masked from ‘package:tidyr’:

    expand, smiths

The following object is masked from ‘package:dplyr’:

    rename

The following objects are masked from ‘package:plyr’:

    rename, round_any

Loading required package: DBI
Loading required package: methods
gdata: read.xls support for 'XLS' (Excel 97-2004) files ENABLED.

gdata: read.xls support for 'XLSX' (Excel 2007+) files ENABLED.

Attaching package: ‘gdata’

The following objects are masked from ‘package:dplyr’:

    combine, first, last

The following object is masked from ‘package:stats’:

    nobs

The following object is masked from ‘package:utils’:

    object.size

The following object is masked from ‘package:base’:

    startsWith

           used  (Mb) gc trigger   (Mb)  max used   (Mb)
Ncells  1406020  75.1    2637877  140.9   2371954  126.7
Vcells 75049058 572.6  175164765 1336.5 145895470 1113.1
There were 50 or more warnings (use warnings() to see the first 50)
[1] TRUE

```

# Provider_PAC_Rates table.sql

```
mysql> use Wellpoint_54005New20170409;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> source Provider_PAC_Rates table.sql
Query OK, 120282 rows affected (1.26 sec)
Records: 120282  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.21 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 12825 rows affected (1.39 sec)
Records: 12825  Duplicates: 0  Warnings: 0

Query OK, 3904 rows affected (1.19 sec)
Records: 3904  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.15 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.16 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.16 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 16700 rows affected (1.57 sec)
Records: 16700  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

```

# HCI3_Reliability_Analysis.R 

```
ubuntu@Cert:/ecrfiles/git/prometheus_distribution/ecrfiles/post_ec/RSPR$Rscript HCI3_Reliability_Analysis.R 
Loading required package: methods
Loading required package: stats4
Loading required package: splines

Attaching package: ‘dplyr’

The following objects are masked from ‘package:plyr’:

    arrange, count, desc, failwith, id, mutate, rename, summarise,
    summarize

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union


Attaching package: ‘tidyr’

The following object is masked from ‘package:VGAM’:

    fill

Loading required package: DBI

Attaching package: ‘car’

The following object is masked from ‘package:dplyr’:

    recode

The following object is masked from ‘package:VGAM’:

    logit

Warning messages:
1: In .local(conn, statement, ...) :
  Decimal MySQL column 4 imported as numeric
2: In .local(conn, statement, ...) :
  Decimal MySQL column 5 imported as numeric
Error in vglm.fitter(x = x, y = y, w = w, offset = offset, Xm2 = Xm2,  : 
  could not obtain valid initial values. Try using 'etastart', 'coefstart' or 'mustart', else family-specific arguments such as 'imethod'.
In addition: There were 15 warnings (use warnings() to see them)
There were 33 warnings (use warnings() to see them)
  Episode_ID level_assignment Attributed_Provider Number_of_Episodes
1     EA0101                1         !0000046348                 15
  Number_of_Epis_w_PAC  PAC_Rate N_Pred Pred_Prob Exp_PAC_Rate        OE
1                   11 0.7333333     15  11.56597    0.7710647 0.9510227
  Provider_Specific_Error Reliability
1                   0.013           0
           alpha             beta     ptp_variance episode_pac_rate 
    5.436336e+09     2.003020e+09     0.000000e+00     7.308000e-01 

EA0101 EA0403 EA0506 EA0610 EC0202 EC0301 EC0401 EC0402 EC0508 EC0511 EC0518 
     1      5      1      5     81    130    108     17     32    188     33 
EC0521 EC0601 EC0611 EC0612 EC0801 EC0802 EC1001 EC1903 EC1906 EC1908 EC1909 
    15     70      7      6    130     59     92      8      2     69    238 
EC1910 EP0202 EP0301 EP0509 EP0510 EP0520 EP0601 EP0602 EP0603 EP0604 EP0610 
    54     16     15      1      1      1    128      1    158      9      6 
EP0811 EP0812 EP0813 EP0816 EP0902 EP0904 EP1202 EP1301 EP1403 EP1404 
    22     12      8      2     26      5      1      8     22      5 
  Episode_ID level_assignment Attributed_Provider Number_of_Episodes
1     EA0101                1         !0000046348                 15
2     EA0403                1         !0000046348                 17
3     EA0403                1         !0000063483                 13
4     EA0403                1         !0000138047                 14
5     EA0403                1         !0000138109                 10
6     EA0403                1         !0000146815                 15
  Number_of_Epis_w_PAC  PAC_Rate N_Pred Pred_Prob Exp_PAC_Rate        OE
1                   11 0.7333333     15 11.565970    0.7710647 0.9510227
2                   10 0.5882353     17  9.115036    0.5361786 1.0970226
3                    7 0.5384615     13  7.385462    0.5681125 0.9478757
4                   12 0.8571429     14  9.217138    0.6583670 1.3018575
5                    3 0.3000000     10  3.895577    0.3895577 0.7701041
6                    4 0.2666667     15  6.336289    0.4224193 0.6313632
  Provider_Specific_Error Reliability
1                  0.0130      0.0000
2                  0.0142      0.6687
3                  0.0191      0.6001
4                  0.0087      0.7672
5                  0.0210      0.5772
6                  0.0130      0.6880
[1] TRUE
[1] TRUE

```


# Master_IEVA_W_Description.sql

```
mysql> use Wellpoint_54005New20170409;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> source Master_IEVA_W_Description.sql;
Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.04 sec)

Query OK, 0 rows affected (0.03 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.02 sec)

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.01 sec)

Query OK, 0 rows affected, 1 warning (0.02 sec)

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.05 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.00 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.04 sec)
Records: 0  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected, 1 warning (0.01 sec)

Query OK, 0 rows affected, 1 warning (0.02 sec)

Query OK, 0 rows affected (0.02 sec)

Query OK, 0 rows affected, 1 warning (0.03 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (14 min 22.20 sec)

Query OK, 0 rows affected (14 min 22.20 sec)

Query OK, 0 rows affected (14 min 22.30 sec)

Query OK, 0 rows affected (14 min 22.32 sec)

Query OK, 0 rows affected (14 min 22.34 sec)

Query OK, 0 rows affected (14 min 22.36 sec)

Query OK, 0 rows affected (14 min 22.39 sec)

Query OK, 0 rows affected (14 min 22.42 sec)

Query OK, 0 rows affected (14 min 22.44 sec)

Query OK, 0 rows affected (14 min 22.46 sec)

Query OK, 0 rows affected (14 min 22.48 sec)

```

# pac_super_groups.sql




```
mysql> use Wellpoint_54005New20170409;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> source pac_super_groups.sql;
Query OK, 0 rows affected (0.03 sec)

Query OK, 677048 rows affected, 65535 warnings (1 min 46.53 sec)
Records: 677048  Duplicates: 0  Warnings: 68908

```





    

	