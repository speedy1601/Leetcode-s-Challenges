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
|   9   | [Rising Temperature](https://leetcode.com/problems/rising-temperature/description/) | [Solution](https://leetcode.com/problems/rising-temperature/solutions/5909035/pandas-polars-postgresql) | `sort_values(), diff(), 'Timedelta()`| `sort(), diff(), duration()` | `INTERVAL (timeseries data)`|
|   10  | [Average Time Of Process Per Machine](https://leetcode.com/problems/average-time-of-process-per-machine/description/) | [Solution](https://leetcode.com/problems/average-time-of-process-per-machine/solutions/5925007/pandas-polars-postgresql) | `round(), sub()` | `round(), sub()` | `ROUND(), INNER JOIN on 4 conditions` |
|   11  | [Employee Bonus](https://leetcode.com/problems/employee-bonus/description/) | [Solution](https://leetcode.com/problems/employee-bonus/solutions/5932212/pandas-polars-postgresql) | | | |
|   12  | [Students And Examinations](https://leetcode.com/problems/students-and-examinations/description/) | [Solution](https://leetcode.com/problems/students-and-examinations/solutions/5938990/pandas-polars-postgresql) | `merge(how='cross')` | `join(how='cross')` | `CROSS JOIN, COUNT(a column)` |
|   13  | [Managers With At Least 5 Direct Reports](https://leetcode.com/problems/managers-with-at-least-5-direct-reports/description/) | [Solution](https://leetcode.com/problems/managers-with-at-least-5-direct-reports/solutions/5942105/pandas-polars-postgresql) | `.agg()` | `.agg()` | `HAVING` |
|   14  | [Confirmation Rate](https://leetcode.com/problems/confirmation-rate/description/) | [Solution](https://leetcode.com/problems/confirmation-rate/solutions/5946527/pandas-polars-postgresql) | | | |
|   15  | [Not Boring Movies](https://leetcode.com/problems/not-boring-movies/description/) | [Solution](https://leetcode.com/problems/not-boring-movies/solutions/5949203/pandas-polars-postgresql) | | | |
|   16  | [Average Selling Price](https://leetcode.com/problems/average-selling-price/description/) | [Solution](https://leetcode.com/problems/average-selling-price/solutions/5953506/pandas-polars-postgresql) | | | |
|   17  | [Project Employees I](https://leetcode.com/problems/project-employees-i/description/) | [Solution](https://leetcode.com/problems/project-employees-i/solutions/5954215/pandas-polars-postgresql) | | | |
|   18  | [Percentage Of Users Attended A Contest](https://leetcode.com/problems/percentage-of-users-attended-a-contest/description/) | [Solution](https://leetcode.com/problems/percentage-of-users-attended-a-contest/solutions/5957003/pandas-polars-postgresql) | | | |
|   19  | [Queries Quality And Percentage](https://leetcode.com/problems/queries-quality-and-percentage/description/?envType=study-plan-v2&envId=top-sql-50) | [Solution](https://leetcode.com/problems/queries-quality-and-percentage/solutions/5957170/pandas-polars-postgresql) | | | |
|   20  | [Monthly Transactions I](https://leetcode.com/problems/monthly-transactions-i/description/) | [Solution](https://leetcode.com/problems/monthly-transactions-i/solutions/5962275/pandas-polars-postgresql) | `agg()` | | `FILTER()` |
|   21  | [Immediate Food Delivery II](https://leetcode.com/problems/immediate-food-delivery-ii/description/) | [Solution](https://leetcode.com/problems/immediate-food-delivery-ii/solutions/5970239/pandas-polars-postgresql) | | | `subquery => WHERE (...) IN (...)` |
|   22  | [Game Play Analysis IV](https://leetcode.com/problems/game-play-analysis-iv/description/) | [Solution](https://leetcode.com/problems/game-play-analysis-iv/solutions/5996925/pandas-polars-postgresql) | `groupby() [..].transform()` | `over(partion_by)` | `OVER (PARTITION BY)` |
|   23  | [Number Of Unique Subjects Taught By Each Teacher](https://leetcode.com/problems/number-of-unique-subjects-taught-by-each-teacher/description/) | [Solution](https://leetcode.com/problems/number-of-unique-subjects-taught-by-each-teacher/solutions/6001679/pandas-polars-postgresql) | | | |
|   24  | [User Activity For The Past 30 Days I](https://leetcode.com/problems/user-activity-for-the-past-30-days-i/description/) | [Solution](https://leetcode.com/problems/user-activity-for-the-past-30-days-i/solutions/6003219/pandas-polars-postgresql) | `pd.Timestamp, pd.to_datetime, between` | `pl.datetime, is_between` | `BETWEEN, ::DATE` |
|   25  | [Product Sales Analysis III](https://leetcode.com/problems/product-sales-analysis-iii/description/) | [Solution](https://leetcode.com/problems/product-sales-analysis-iii/solutions/6007319/pandas-polars-postgresql) | `filter()` | | |
|   26  | [Classes More Than 5 Students](https://leetcode.com/problems/classes-more-than-5-students/description/) | [Solution](https://leetcode.com/problems/classes-more-than-5-students/solutions/6007625/pandas-polars-postgresql) | `groupby(.., as_index = False)` | | |
|   27  | [Find Followers Count](https://leetcode.com/problems/find-followers-count/description/) | [Solution](https://leetcode.com/problems/find-followers-count/solutions/6007866/pandas-polars-postgresql) | | | |
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
| 9 | How to INNER `JOIN` based ON `ASSUMED columns` but behind the scene the original table's values remain as they are. Also `ITS VERY IMPORTANT TIME related Q` |
| 10| How do INNER `JOIN` actually works and we can do `split a dataframe into two and INNER JOIN them` with A SINGLE INNER JOIN on that dataframe |
| 12| How `group by` handles `NULL` values while grouping in Pandas, Polars, PostgreSQL |
| 13| In `PANDAS, POSTGRESQL` you can perform `AGGREGATE FUNCTIONS` on the `GROUPING KEYS` but in `POLARS` you can't |
| 14| Instead of `(df['active'] == 'Yes').sum() / df['active'].size()` just do `(df['active'] == 'Yes').mean()` |
| 16| If your information has inside 2 tables, JOIN them anyhow, even by their primary key, even if you don't get your desired mixed table because you can filter that mixed table and then get your desired table|
| 19| Sometimes in your `Pandas or Polars` code, before rounding up a Float value to CERTAIN DECIMAL NUMBERS, you might need to add `1e-10` to the FLOAT value first |
| 20| In `Pandas` if your solution needs only aggregrate functions like `count(), sum()`, use `agg()` even if you've to create some more columns, don't use `apply()` in this case. In `PostgreSQL` `GROUP BY` clause can access the `alias` created in `SELECT` as like `NEW COLUMN OF THAT TABLE` and can perform GROUP BY on that alias |
| 22| `THINK SIMPLY`. JUST CREATING A NEW COLUMN can save your time, optimize efficiency and just more creative. (`IMPORTANT TRICKY QUESTION`). And in `POSTGRESQL` you can't perform `NESTED AGGREGATE FUNCTION` during `GROUP BY operation` and also you can't do `player_id = MIN(player_id)` without using `player_id in group by` |
| 26 | In `PANDAS`, `groupby(by=.., as_index=False) .agg(..)` returns A DataFrame. So no need to do `reset_index` anymore unless necessery |