# Azure Data Explorer Analysis Guidelines

## Query Sharing

1. Always provide a link to the query you ran for Azure Data Explorer web. Create the link through this pattern:
   ```
   https://dataexplorer.azure.com/clusters/{clusterName}/databases/{databaseName}?query={urlEncodedQuery}
   ```
   This allows others to easily reproduce and modify your analysis.

## Result Presentation

2. Provide the query results as a table in a collapsible segment:
   ```markdown
   <details>
   <summary>Query Results</summary>

   | Column1 | Column2 | Column3 |
   |---------|---------|---------|
   | Value1  | Value2  | Value3  |
   | ...     | ...     | ...     |
   
   </details>
   ```

## Analysis Structure

3. Follow the results with thorough analysis and summary, focusing on:
   - User engagement metrics (2d28 - users active 2 days in 28 day period)
   - Highly engaged users (10d28 usage - users active 10+ days in 28 day period)
   - Retention metrics and patterns
   - Growth-hacking opportunities
   - Suggestions for additional analysis avenues

## Example Analysis Template

```markdown
## Analysis of [Metric Name]

### Key Findings
- Finding 1
- Finding 2
- Finding 3

### User Engagement Patterns
[Describe engagement patterns observed in the data]

### Retention Insights
[Analyze user retention metrics and patterns]

### Growth Opportunities
[Identify potential growth-hacking opportunities]

### Suggested Further Analysis
- Suggestion 1
- Suggestion 2
- Suggestion 3
```