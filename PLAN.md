# HW 4.3 Project and Repo Plan

## Part 1 — Project Plan

### Goals

My main goal is to put my HW 4.3 work into one Quarto report. Someone should be able to download the repo and render the report.

I have four smaller goals.

- Compare diamond length, width, and height across clarity groups.
- Show Penn State women's basketball scores for the 2025–26 season.
- Use random points to estimate the area under a Weibull curve.
- Compare the calcium plot based on my plan with the generic plot.

### Needs

#### Software and R Packages

- R and RStudio to work with the code.
- Quarto to render the report.
- tidyverse to organize data and make plots.
- knitr to make tables and generate the code appendix.

#### Files and Data

- 4.3.qmd for the report text and code.
- 4.3.pdf for the saved report.
- The diamonds dataset from ggplot2.
- team_box.csv for the basketball analysis.
- calcium_plan_plot.png for the plot based on my plan.
- chatgptPlot.png for the generic comparison plot.
- The assignment instructions and feedback on my earlier work.

### Steps

#### Set Up the Report

1. Gather my earlier assignments, data, and images.
2. Keep the QMD and its input files in the same project folder.
3. Add a YAML header at the top of the QMD.
4. Include a title, my name, a date, and the output format.
5. Set the report to produce a PDF.
6. Set code options so the main report shows the results clearly.
7. Load the R packages in the first code chunk.
8. Add a comment near the top to name the coding style I follow.

#### Prepare the Diamond Tables

9. Start with the diamonds dataset from ggplot2.
10. Remove rows with a zero length, width, or height.
11. Keep clarity and the three dimension columns.
12. Put the dimension measurements into a long format.
13. Group the data by dimension and clarity.
14. Calculate the count, percentiles, median, mean, and standard deviation.
15. Make separate tables for length, width, and height.
16. Give each table a clear caption.
17. Describe the main patterns in short paragraphs.
18. Check unusual values before discussing them.

#### Prepare the Basketball Plot

19. Read team_box.csv with a relative file path.
20. Check that the columns needed by the code are present.
21. Keep Penn State records for the 2025–26 season.
22. Check for missing dates and scores.
23. Check for repeated game records.
24. Keep one record for each Penn State game.
25. Sort the games by date.
26. Count the wins and losses.
27. Plot points scored against points allowed.
28. Add a dashed line where points scored equal points allowed.
29. Connect the games in date order.
30. Add axis labels, a caption, and alt text.
31. Check that the win and loss counts agree with the plotted data.
32. Explain what the points and lines show.

#### Prepare the Monte Carlo Simulation

33. Define the Weibull curve and the sampling rectangle.
34. Use the same rectangle for all sample sizes.
35. Set random seeds so the results can be repeated.
36. Generate 10, 100, 1,000, and 10,000 random points.
37. Mark whether each point falls on or below the curve.
38. Find the share of points on or below the curve.
39. Multiply that share by the rectangle's area.
40. Show the four plots together.
41. Give the plots captions and alt text.
42. Compare the estimates with the exact area.
43. Explain how the sample size affects the estimates.

#### Compare the Calcium Plots

44. Add the plot based on my analysis plan.
45. Add the generic plot provided with the assignment.
46. Explain the groups and measurement times.
47. Check the group means shown in the table.
48. Compare how the two plots organize the measurements.
49. Explain what I can learn from each plot.
50. Describe any limits of comparing group averages.

#### Finish and Check the Report

51. Use clear headings to separate the sections.
52. Keep the written explanations outside the code chunks.
53. Give each code chunk a unique label.
54. Check captions and alt text for figures.
55. Use the same coding style throughout the report.
56. Generate the code appendix from the analysis chunks.
57. Keep Chinese code comments out of the rendered PDF.
58. Review the AI usage appendix and describe the help I used.
59. Render the QMD from a fresh R session.
60. Fix any missing-file errors.
61. Check that all tables and figures appear in the PDF.
62. Check page breaks and look for text that runs off the page.
63. Check that the written results match the tables and figures.
64. Save the final QMD and PDF.

## Part 2 — GitHub Repo Plan

### Goals

My main goal is to keep a public repo that the grading team can open.

The repo should contain the report and all its input files. The README should help readers find the files and understand the project.

I also want to use branches, issues, commits, and pull requests to track my work.

### Needs

- My GitHub account.
- A public repo made from the class template.
- A main branch and a dev branch.
- Two issues with useful labels.
- My report, data, and images.
- A README and a separate plan file.
- Clear commit messages.
- A pull request to merge my work into main.

### Steps

#### Set Up the Repo

1. Create a public repo from the class template.
2. Check that the repo belongs to my account.
3. Check that main is the default branch.
4. Create dev from main.
5. Open an issue for adding the report and input files.
6. Give that issue the enhancement label.
7. Open an issue for the README and project plan.
8. Give that issue the documentation label.

#### Add the Files

9. Switch to dev before making changes.
10. Upload the QMD and PDF.
11. Upload team_box.csv as a CSV file.
12. Upload both calcium images.
13. Keep input files where the QMD expects to find them.
14. Check that file names match the names used in the code.
15. Use relative paths for files in the repo.
16. Commit the report files with a clear summary.
17. Reference the report issue in the commit message.
18. Replace the README template text with my project information.
19. List the data sources and acknowledge help I used.
20. Explain the current plan and the repo structure.
21. Include my name and a way to contact me through GitHub Issues.
22. Commit the README update.
23. Add PLAN.md with goals, needs, and steps for both parts of the work.
24. Commit the plan and reference the documentation issue.

#### Review and Merge

25. Open a pull request with main as the base and dev as the compare branch.
26. Give the pull request a clear title.
27. Explain what the changes add and why they are needed.
28. Reference the issues that the changes complete.
29. Review the changed files.
30. Check that the report and its inputs are included.
31. Merge the pull request into main.
32. Check that the completed issues are closed.
33. Keep dev for future changes.
34. Check that main contains the latest report and documents.

#### Check the Submission

35. Open the repo homepage.
36. Confirm that the repo is public.
37. Open the PDF and check that it loads.
38. Open the QMD and check that the source is available.
39. Check that the CSV and images are present.
40. Check that the README links and file names are correct.
41. Submit the repo homepage URL in the assignment.

### Future Maintenance

For a new task, I will open an issue or update an existing one. I will make changes on dev and use a clear commit message.

Before merging, I will review the changes. If the analysis changes, I will render the report again and update the PDF.

After merging, I will check that main has the latest files. I will close an issue when its task is finished.
