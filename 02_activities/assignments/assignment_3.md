# Data Visualization

## Assignment 3: Final Project

### Requirements:
- We will finish this class by giving you the chance to use what you have learned in a practical context, by creating data visualizations from raw data. 
- Choose a dataset of interest from the [City of Toronto’s Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/) or [Ontario’s Open Data Catalogue](https://data.ontario.ca/). 
- Using Python and one other data visualization software (Excel or free alternative, Tableau Public, any other tool you prefer), create two distinct visualizations from your dataset of choice.  

Data Souce: https://data.ontario.ca/dataset/live-births-by-age-of-parents/resource/8b493432-a9cf-4d80-ae46-8378213d8438

- For each visualization, describe and justify: 
    > What software did you use to create your data visualization?
    Python and Excel are used to create the data visualization. 
    Before generating graphs, data cleansing was performed in both python and Excel (with power query)

    1. Plotly chart (with Python): an interactive vertical bar chart showing the distribution of father age groups for underage mothers, providing hover tooltips and exported the visualization as an interactive HTML file
    2. Excel chart: line chart showed the annual trend in birth counts among underage mothers (≤17 years old) from 2012 to 2023. Linear trendline and equation are added in the graph to clearly indicate a downward trend to audience, and for further study by statisticians if interested

    > Who is your intended audience? 
    Public health officials, policymakers, educators and social researchers who are concerned with adolescent health and family planning
    
    1. Public Health Officials: can use the trend analysis (Excel chart) to monitor changes in underage births and design targeted interventions
    2. Policymakers: rely on the data to inform legislation or resource allocation for youth support programs
    3. Educators: use the insights to strengthen awareness campaigns and prevention strategies
    4. Researchers: may benefit from the interactive plot as it helps analyze how father age groups are associated with underage mothers over time, which is important information for studying social dynamics, identifying risk factors (e.g.if underage mother paired with much older father may raise concern about power imbalances) and informing public health and policy discussion
 
    > What information or message are you trying to convey with your visualization? 
    - Excel chart: show trend - the number of births to underage mothers (≤17 years old) has been steadily decline from 2012 to 2023 (with strong linear decrease)
    - Interactive plot: show distribution - which father age groups are most common among underage mothers, helping to reveal social patterns and potential risk factors
    - Both visualizations aim to understand and help social and public health implications

    > What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots? 
    1. Choice of Graph: 
    - Line Chart: it is the most effective way to show a trend over time, the line emphasize a steady decline in underage birth throughout years, and the added trendline with equation and  
    R² value quantifies the strength of this downward pattern. Other chart types (such as pie charts or bar charts) wouldn't convey as clear as line chart
    - Vertical Bar Chart in Plotly: bar chart is ideal for comparing categories side by side, allow audiences easy to see which father age groups are more common among underage mothers. Other charts (such as line chart or scatterplot) would have been less intuitive for categorical comparison. When compared with pie chart, bar chart is better for showing exact birth counts across categoris while pie chart emphasizes percentage (harder to interpret when categoris are close in size).
        - hover tooltips and zomming functions are included in the visualization so that audience can interact with the graph if they want to explore data dynamically
    2. Readability: precise titles and clear axis labels are added to let audience immediately undestand the chart. Dashed gridlines are included to improve the intuitive clarity.
    3. Design: Stylish font in main chart title is designed to draw attention. Contrastng colors (Excel: blue line with yellow labels; Plotly: blue bar with white background, and orange dashed gridline) are used so that data points stand out clearly and keep the charts visually appealing. The strong contrast avoid the common red/green pairing (difficult for many viewers)and the included data labels and hover tooltips improve accessibility and avoid information conveyed only by color. 


    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization? 
    I ensure reproducibility by using Power Query in Excel and Python scripts with Plotly.
    - Power Query records each data cleaning step, so anyone opening the workbook can refresh and automatically apply the same transformation (e.g. handling N.S. and N.P. values as "Unknown")
    - Python has an even stronger reprocibility as the code documents every step of the process, allowing others to both rerun the script and verify the logic. Comparing Power Query, steps are less transparent as Python because the logic are not as clearly stated unless people open the query editor and follow every step.
    - Since the visualization was based on deterministic data cleaning and plotting, no random sampling or simulation were involved, a seed (np.random.seed(613)) was not include to ensure reproducibility across runs

    If a tool doesn't support reproducibility (e.g. manual Excel formating without clear documentation), the visualization may be harder to reproduce consistently and the process is less transparent and less verifiable. 

    > How did you ensure that your data visualization is accessible?
    I ensure accessibility by using clear titles, readable fonts, and high-contrast colors (aforementioned). Added data labels and hover tooltips so information is not conveyed by color alone, and chose simple backgrounds to keep charts uncluttered. Interactivity of plotly also make visualization easier to explore for difference audiences.  
    
    > Who are the individuals and communities who might be impacted by your visualization?  
    Apart from Public health officials, policymakers, educators and social researchers that have already covered in previous questions:
    - Underage mothers and their children might be impacted by the visualization: as it reveals their life experiences to public
    - Healthcare providers such as doctors, nurses etc: get the insights to anticipate health needs of young mother and their infants
    - Social workers and conselors & Legal and child protection agencies: understand age dynamics between parents to tailor support services
    - General Public: raise awareness 

    > How did you choose which features of your chosen dataset to include or exclude from your visualization? 
    I chose features based on their relevance to the story I wanted to tell.
    I included mother's age (≤17 years) and father's age group because they directly highlight the decline in underage births and age dynamics between parents.
    For missing values like N.S. and N.P,  cleaned the data using consistent rules, retaining them as "Unknown" rather than discarding them. This ensure transparency and avoid bias from excluding cases. 
    
    > What ‘underwater labour’ contributed to your final data visualization product?
    1. Data Cleaning: dealt with messy values by transforming them into "Unknown" in both platform to ensure consistency and transparency
    2. Data Preparation: grouped and filtered the dataset to focus on mothers ≤17 and grouped fathers into age categories, which require careful data exploration and structuring before visualization
    3. Design Iteration: tested different chart types and refine choices based on clarity and suitability 
    4. Accessibility Adjustments: added labels, hover tooltips etc. to ensure charts were accessible to diverse audiences
    5. Verification: cross-checked outputs between Excel and Python to confirm that the trends and counts matched, reducing the risk of errors

- This assignment is intentionally open-ended - you are free to create static or dynamic data visualizations, maps, or whatever form of data visualization you think best communicates your information to your audience of choice! 
- Total word count should not exceed **(as a maximum) 1000 words** 
 
### Why am I doing this assignment?:  
- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes: 
* Create and customize data visualizations from start to finish in Python
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story  
- This would be a great project to include in your GitHub Portfolio – put in the effort to make it something worthy of showing prospective employers!

### Rubric:

| Component         | Scoring  | Requirement                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| Data Visualizations | Complete/Incomplete | - Data visualizations are distinct from each other<br>- Data visualizations are clearly identified<br>- Different sources/rationales (text with two images of data, if visualizations are labeled)<br>- High-quality visuals (high resolution and clear data)<br>- Data visualizations follow best practices of accessibility |
| Written Explanations | Complete/Incomplete | - All questions from assignment description are answered for each visualization<br>- Explanations are supported by course content or scholarly sources, where needed |
| Code              | Complete/Incomplete | - All code is included as an appendix with your final submissions<br>- Code is clearly commented and reproducible |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 02/23/2026`
* The branch name for your repo should be: `assignment-3`
* What to submit for this assignment:
    * A folder/directory containing:
        * This file (assignment_3.md)
        * Two data visualizations 
        * Two markdown files for each both visualizations with their written descriptions.
        * Link to your dataset of choice.
        * Complete and commented code as an appendix (for your visualization made with Python, and for the other, if relevant) 
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-3`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
