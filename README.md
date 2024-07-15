# week-3
*DISCLAIMER
The following are Answers based on the imported Expenses.mql data in LMS, in week 3 learning material in the Google drive.
# Week 3: Grouping Your Expenses for Smarter Spending

Let's Practice! (2 hours)

## Challenges:

**1.1.** Total Spent per Category: 
Write a query to find the total amount you spent in each category (Groceries, Entertainment, etc.). Hint: Use GROUP BY category and SUM (amount).

SELECT category, SUM(amount) AS total¬_spent
FROM myexpenses1_cleaned 
GROUP BY category;

Results
Alone 2710
Friend 1889

**1.2.** Average Expense per Category: 
Now, let's see the average cost for each category. Write a query to find the average expense amount for each category. Hint: Use GROUP BY category and AVG (amount).


SELECT category, AVG(amount) AS average_expense
FROM myexpenses1_cleaned
GROUP BY category;

Results
Alone 29.78
Friend 35.64


## Bonus Challenge (Optional): 
Are you curious about your top spending categories? Modify your query from Challenge 1 to show only the top 3 (or a chosen number) categories where you spend the most.
**Remember:**
There might be different ways to solve these chal


SELECT category, SUM(amount) AS total_spent
FROM myexpenses1_cleaned
GROUP BY category
ORDER BY total_spent DESC
LIMIT 3;

Results
Alone 2710
Friend 1889



