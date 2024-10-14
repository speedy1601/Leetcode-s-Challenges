50 Easy to Intermediate SQL Qs from [Top SQL 50](https://leetcode.com/studyplan/top-sql-50/)
I solved each question using Pandas, Polars, PostgreSQL.

|   No  |   Question  |  Solution   | Methods Used (pandas) | Methods Used (polars) | Methods Used (postgreSQL, except SELECT and FROM) |
| :---- | :-----------| :---------- | :---------------------| :---------------------| :-------------------------------------------------|
|   1   | [Recyclable and Low Fat Products](https://leetcode.com/problems/recyclable-and-low-fat-products/description/?envType=study-plan-v2&envId=top-sql-50) | [Solution](https://leetcode.com/problems/recyclable-and-low-fat-products/solutions/5896967/pandas-polars-and-postgresql) | `loc[]` | `filter(), select()` | `WHERE`|
|   2   | [Find Customer Referee](https://leetcode.com/problems/find-customer-referee/description/) | [Solution](https://leetcode.com/problems/find-customer-referee/solutions/5898178/pandas-polars-and-postgresql) | | | `ISNULL, COALESCE` |
|   3   | [Big Countries](https://leetcode.com/problems/big-countries/) | [Solution](https://leetcode.com/problems/big-countries/solutions/5898265/pandas-polars-postgresql) | | | |
|   4   | [Article Views I](https://leetcode.com/problems/article-views-i/description/) | [Solution](https://leetcode.com/problems/article-views-i/solutions/5898437/pandas-polars-postgresql) | `drop_duplicates(), sort_values(), rename()` | `unique(), sort(), rename()` | `DISTINCT, ORDER BY` |
|   5   | [Invalid Tweets](https://leetcode.com/problems/invalid-tweets/description/?envType=study-plan-v2&envId=top-sql-50) | [Solution](https://leetcode.com/problems/invalid-tweets/solutions/5898689/pandas-polars-postgresql) | `str.len()` | `str.len_chars()`| `LENGTH()` |
|   6   | [Replace Employee Id With The Unique Identifier](https://leetcode.com/problems/replace-employee-id-with-the-unique-identifier/description/) | [Solution](https://leetcode.com/problems/replace-employee-id-with-the-unique-identifier/solutions/5903096/pandas-polars-postgresql) |`merge(how='left')`|`join(how='left')` |`LEFT JOIN` |
|   7   | [Product Sales Analysis I](https://leetcode.com/problems/product-sales-analysis-i/description/?envType=study-plan-v2&envId=top-sql-50) | [Solution](https://leetcode.com/problems/product-sales-analysis-i/solutions/5903591/pandas-polars-postgresql) |`merge(how='inner'), drop(columns), iloc[]` |`join(how='inner'), drop(columns), pl.col('*').exclude()` | `INNER JOIN, subquery` |
|   8   | [Customer Who Visited But Did Not Make Any Transactions](https://leetcode.com/problems/customer-who-visited-but-did-not-make-any-transactions/description/) | [Solution](https://leetcode.com/problems/customer-who-visited-but-did-not-make-any-transactions/solutions/5907523/pandas-polars-postgresql) |`isin(), groupby(), reset_index()` | `is_in(), group_by()` | `group by, count(*)`|
|   9   | [Rising Temperature](https://leetcode.com/problems/rising-temperature/description/) | [Solution](https://leetcode.com/problems/rising-temperature/solutions/5909035/pandas-polars-postgresql) | `sort_values(), diff()`| `sort(), diff()` | `INTERVAL (timeseries data)`|
|   10  | []() | []() | | | |
|   11   | []() | []() | | | |
|   12   | []() | []() | | | |
|   13   | []() | []() | | | |
|   14   | []() | []() | | | |
|   15   | []() | []() | | | |
|   16   | []() | []() | | | |
|   17   | []() | []() | | | |
|   18   | []() | []() | | | |
|   19   | []() | []() | | | |
|   20   | []() | []() | | | |
|   21   | []() | []() | | | |
|   22   | []() | []() | | | |
|   23   | []() | []() | | | |
|   24   | []() | []() | | | |
|   25   | []() | []() | | | |
|   26   | []() | []() | | | |
|   27   | []() | []() | | | |
|   28   | []() | []() | | | |
|   29   | []() | []() | | | |
|   30   | []() | []() | | | |
|   31   | []() | []() | | | |
|   32   | []() | []() | | | |
|   33   | []() | []() | | | |
|   34   | []() | []() | | | |
|   35   | []() | []() | | | |
|   36   | []() | []() | | | |
|   37   | []() | []() | | | |
|   38   | []() | []() | | | |
|   39   | []() | []() | | | |
|   40   | []() | []() | | | |
|   41   | []() | []() | | | |
|   42   | []() | []() | | | |
|   43   | []() | []() | | | |
|   44   | []() | []() | | | |
|   45   | []() | []() | | | |
|   46   | []() | []() | | | |
|   47   | []() | []() | | | |
|   48   | []() | []() | | | |
|   49   | []() | []() | | | |
|   50   | []() | []() | | | |

There are some questions helped me to strong the base :
| Question No | Description |
| :---------- | :---------- |
| 6 | How to keep all the `NULL VALUES` at the very `FIRST OR LAST` without sorting the other NON NULL values. |
| 9 | How to INNER `JOIN` based ON `ASSUMED columns` but behind the scene the original table's values remain as they are. |