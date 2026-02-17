# Data Visualization

## Assignment 2: Good and Bad Data Visualization

### Requirements:

- Data visualizations are important tools for communication and convincing; we need to be able to evaluate the ways that data are presented in visual form to be critical consumers of information 
- To test your evaluation skills, locate two public data visualizations online, one good and one bad  
    - You can find data visualizations at https://public.tableau.com/app/discover or https://datavizproject.com/, or anywhere else you like! 
- For each visualization (good and bad):  
    - Explain (with reference to material covered up to date, along with readings and other scholarly sources, as needed) why you classified that visualization the way you did.
      ```
      For example of a Good Data Visualization: Daniel Foster's CO2 Emissions Over Time ![alt text](image.png)
      - Perceptual and Substantive: Line charts fit time-series data, and make trends easy to follow
      - Clear title and labels, and simple designs to avoid clutter (reference: Tufte)
      - Aesthetic: Colors are distinct and consistent, aiding readibility
      - When hover over each location on the map it can show the name of location and its CO2 per capita, aiding exploration


      For example of a Bad Data Visualiztion: Ian's Toronto Blue Jays Home Runs ![alt text](image-1.png)

      - Substantive: it does not accurately represent the data as y-axis "Running Sum of Home Runs" implies a cumulative progression over time/the game, but the bars show each player's contribution stacked into total
      - Lack of clear message: it fails to communicate a central insight - the stacking and last column's "total" running of the whole team make it unclear whether the goal is to highlight individual contribution or the team's total
      --> cause audience confusion, and fail to "tell a story" from this visualization (reference: Cairo)
      - Accessibility: the chart relies on a single color (blue) without visual cues, such as adding label on each bar, which makes it less intuitive




      ```
    - How could this data visualization have been improved?  
      ```
      For the good one:
      - Can add some annotations for key climate events, such as the Kyoto Protocol or Paris Agreement
      - Though the graph consists of red, orange and blue gradients, it is moderately color-blind friendly, while there maybe blue-yellow blindness viewers which red/orange tones are too close in brightness, using palettes with high contrast such as blue-orange only might improve the visualization accessibility (reference: WCAG)
      - Provide a short caption to guid non-expert viewers

      For the bad one:
      - Switch to use a standard bar chart to show each player's home runs side by side
      - Label each bar directly with the player's total to avoid confusion
      - Add a clear title/subtitle emphasizing the team's overall lead in MLB home runs, while keeping the chart focused on player contributions
      - if the author's goal is to highlight the "Big three" (ie Donaldson, Bautista and Encarnacion), adding a pie chart shoing their share of the total on the side would be effective

      
      ```
      Reference:
      Tufte, E. R. (1983). The Visual Display of Quantitative Information.
      Cairo, A. (2012). The Functional Art: An Introduction to Information Graphics and Visualization.
      World Wide Web Consortium (W3C). Web Content Accessibility Guidelines (WCAG) 


- Word count should not exceed (as a maximum) 500 words for each visualization (i.e. 
300 words for your good example and 500 for your bad example)

### Why am I doing this assignment?:

- This assignment ensures active participation in the course, and assesses the learning outcomes
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story

### Rubric:

| Component               | Scoring   | Requirement                                                 |
|-------------------------|-----------|-------------------------------------------------------------|
| Data viz classification and justification | Complete/Incomplete | - Data viz are clearly classified as good or bad<br />- At least three reasons for each classification are provided<br />- Reasoning is supported by course content or scholarly sources |
| Suggested improvements  | Complete/Incomplete | - At least two suggestions for improvement<br />- Suggestions are supported by course content or scholarly sources |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 02/16/2026`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (assignment_2.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
