# Multilingual Web Crawler
Crawl Multilingual language News Website Content like VovWorld, VNAnet, VietNamPlus, QuanDoiNhanDan, etc

This tools made by me with help of instructors **Dr. Tran Hong Viet** (thviet79) and **masters Bui Van Tan**

This tool is by for Window and Linux users, it purpose to crawl rare Language such as **Laotian, Khmer** and popular language like **Chinese, English** etc you can add more if you want

First, I'll talk about my Folders and Files organize and how it work. For each website News you have 1 Folder, it contains link of categories manually collected in linkauto Folder. When the tool run it'll check this folder to get all the news link, title (and date) at first run time. At second time etc, it with check the latest news of the website then add it to resource to save time (time it's knowledge and sleep =)).

Second, it's our approach to detecting bilingual news. As you know news has **title and date (some not in numeric format)**. Beacause news is very lagre resource so compare them is very time consuming. So we set ***date range*** around 15 days or 1 month. It reduce a lot of unnecessary canculating. With title we **translate it from Machine translation** (googleApi etc) to translate it to **Vietnamese**. After that titles will be tokenize by **VNCoreNLP** then use **TF-IDF** to compare them similar or not. 
