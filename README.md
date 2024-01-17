# Heights_weights-Project
The data that we must be careful of is small-sized data, and here you must deal with it with caution and precision and demonstrate your skills in analyzing and dealing with it. Here I deal with small and simple data, but carefully .
----------------------------
One of the university subject projects

I read the file easily using the read_csv method and displayed the first 5 rows to see it and understand its features, then I checked the statistical description of the dataset using the describe method to explore the summary statistics and understand more about the data.


After that, I Visualize the dataset to explore it more, trying to find a few patterns, understand it better, and explore the relationship between them. During the visualization, I discovered that there was something strange but I didn't know what it was specifically!

so I decided to see the info about the data and the null values then I discovered that there are null values and I decided to fill it in because it is numerical data and one of the common practices in this case is to fill the null values using the mean.

While filling null values **I find a pattern** in the data!

The data **increases together**, so that when the Height value increases, the Weight value also increases, and vice versa.

Therefore, **the best** thing we can do is to **resorting the data according to the Weight values** in ascending order, and then **fill the null values** so that they take the value of the **one before or after it.**


**Also, I find another pattern** here !!
The data is **not just increasing together**, I found another thing !!
The Weight values accompanying the null values are **duplicates**, meaning that **we can replace the height values precisely by taking the height value that has the same weight as the null values.**

To do that I used the fillna method and gave the parameter 'method' 'ffill' value to fill it forward. **But The value at Index 5** took the value before it, while it should take the value after it, so I modified its value.
