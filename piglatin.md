# Pig Latin Complete Commands with Explanation

Below are some common Pig Latin commands along with explanations:

1. **LOAD**:
   - Syntax:
     ```piglatin
     LOAD 'file_path' [USING function] [AS schema];
     ```
   - Explanation:
     The `LOAD` command is used to load data from a file into a relation. 
     - `'file_path'`: Path to the file containing the data.
     - `USING function`: Optional. Specifies a function to use for loading the data (e.g., `PigStorage(',')` for CSV files).
     - `AS schema`: Optional. Specifies the schema of the relation.

2. **STORE**:
   - Syntax:
     ```piglatin
     STORE relation INTO 'output_path' [USING function];
     ```
   - Explanation:
     The `STORE` command is used to store the contents of a relation into a file.
     - `relation`: The relation whose contents are to be stored.
     - `'output_path'`: Path where the output file will be stored.
     - `USING function`: Optional. Specifies a function to use for storing the data.

3. **FILTER**:
   - Syntax:
     ```piglatin
     filtered_data = FILTER data BY condition;
     ```
   - Explanation:
     The `FILTER` command is used to filter data based on a condition.
     - `data`: Input relation.
     - `condition`: The condition used to filter the data.

4. **FOREACH**:
   - Syntax:
     ```piglatin
     transformed_data = FOREACH data GENERATE expression AS alias;
     ```
   - Explanation:
     The `FOREACH` command is used to apply transformations to each tuple in a relation.
     - `data`: Input relation.
     - `expression`: Transformation expression.
     - `alias`: Alias for the transformed data.

5. **GROUP**:
   - Syntax:
     ```piglatin
     grouped_data = GROUP data BY key;
     ```
   - Explanation:
     The `GROUP` command is used to group data based on a key.
     - `data`: Input relation.
     - `key`: Key based on which the data will be grouped.

6. **JOIN**:
   - Syntax:
     ```piglatin
     joined_data = JOIN relation1 BY key, relation2 BY key;
     ```
   - Explanation:
     The `JOIN` command is used to join two relations based on a common key.
     - `relation1`, `relation2`: Relations to be joined.
     - `key`: Key based on which the join will be performed.

7. **ORDER**:
   - Syntax:
     ```piglatin
     ordered_data = ORDER data BY key [ASC|DESC];
     ```
   - Explanation:
     The `ORDER` command is used to sort data based on a key.
     - `data`: Input relation.
     - `key`: Key based on which the data will be sorted.
     - `ASC|DESC`: Optional. Specifies ascending or descending order.

8. **LIMIT**:
   - Syntax:
     ```piglatin
     limited_data = LIMIT data n;
     ```
   - Explanation:
     The `LIMIT` command is used to limit the number of tuples in a relation.
     - `data`: Input relation.
     - `n`: Number of tuples to limit the relation to.

9. **DESCRIBE**:
   - Syntax:
     ```piglatin
     DESCRIBE relation;
     ```
   - Explanation:
     The `DESCRIBE` command is used to display the schema of a relation.
     - `relation`: The relation whose schema needs to be described.

10. **DUMP**:
    - Syntax:
      ```piglatin
      DUMP relation;
      ```
    - Explanation:
      The `DUMP` command is used to display the contents of a relation.
      - `relation`: The relation whose contents need to be displayed.

These commands are fundamental to writing Pig Latin scripts for data processing in Apache Pig.
