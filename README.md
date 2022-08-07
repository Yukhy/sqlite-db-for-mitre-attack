(日本語で下に記載)
 
# Sqlite DB for MITRE ATT&CK(beta)
*WARNING: It is NOT MITRE's official repository.　I'm not responsible for the accuracy of the data.*  
<br>
 It is a simple sqlite database for mitre-attack. Basic information on Tactics, Techniques and Groups of MITRE ATT&CK V11 is in the database.  
 As a sqlite database, it is suitable for data analysis in Jupyter Notebook, Google Colaboratory, etc.

## How to Use
Place attack.db in any directory.

## Structure of Database
 This database consists of 11 tables.　There are three tables each for tactics and techniques, one table for groups, three join tables connecting tactics and techniques, and one join table connecting groups and techniques.　Tactics, Techniques, and three intermediate tables exist for Enterprise, Mobile, and ICS, respectively.
![ER diagrams](https://i.imgur.com/REHe3RD.png)
- ent_hogehoge: Indicates that this is the table is a hogehoge table of enterprise.
- mbl_hogehoge: Indicates that this is the table is a hogehoge table of mobile.
- ics_hogehoge: Indicates that this is the table is a hogehoge table of ics.
- j_hogehoge_hugahuga: Indicates that this is the join table is between hogehoge and hugahuga.
## Structure of Field
- For Normal tables
![field](https://i.imgur.com/1N7YIqh.png)

- For Join tables
  - Tactics and Techniques
   ![field](https://i.imgur.com/WCcILDK.png)
  - Groups and Techniques
   ![field](https://i.imgur.com/yFMSp7h.png)

## About sample directiory
- convert_db_to_df.ipynb  
  This sample is an example of converting database records into a Pandas Dataframe.
  
---------

# Sqlite DB for MITRE ATT&CK(beta)
*警告: これはMITREの公式リポジトリではありません。　データの正確性について、責任を負いかねます。*

MITRE ATT&CKのデータが格納されたsqliteデータベースです。MITRE ATT&CK V11のTactics, Techniques, Groupsに関しての基本情報が格納されています。  
 sqliteデータベースであるため簡単に、Jupyter NotebookやGoogle Colaboratoryなどで利用できます。

## 使い方
attack.dbを任意のディレクトリに配置してください。

## データベースの構造
 このデータベースは11個のテーブルで構成されています。　内訳はTacticsとTechniquesがそれぞれ3テーブル、Groupsが1テーブル、TacticsとTechniquesをつなぐ中間テーブルが3テーブル、GroupsとTechniquesをつなぐ中間テーブルが1テーブルです。　Tactics、Techniquesのテーブルとそれらの中間テーブルはEnterprise, Mobile, ICSごとに用意されています。
![ER diagram](https://i.imgur.com/rlKLTfb.png)
- ent_hogehoge: enterpriseのテーブルであることを示します。
- mbl_hogehoge: mobileのテーブルであることを示します。
- ics_hogehoge: icsのテーブルであることを示します。
- j_hogehoge_hugahuga: hogehogeとhugahugaの中間テーブルであることを示します。

## テーブルの構造
- 通常のテーブルの場合
   ![field](https://i.imgur.com/xOPpiqr.jpg)

- ジョインテーブルの場合
  - TacticsとTechniques
   ![field](https://i.imgur.com/zlCdu49.png)
  - GroupsとTechniques
   ![field](https://i.imgur.com/yTWZwTF.png)

- サンプルディレクトリについて
  - convert_db_to_df.ipynb  
  本サンプルは、データベースのレコードをPandas Dataframeに変換する例です。
