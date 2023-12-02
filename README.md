# pr-full-report-action

**pr-full-report-action** is a comprehensive tool designed to generate detailed reports on closed pull requests (PRs). This powerful GitHub Action aids in tracking and analyzing the efficiency and productivity of software development workflows.

## Key Features:

- **PR Timeline Analysis**: Generates a table showcasing the time taken from PR opening to the first review, approval, and final merge. This feature helps in understanding the responsiveness and review efficiency within the team.
- **Developer-Specific Metrics**: Calculates and presents both median and average values for each metric, broken down by individual developers. This allows for a granular analysis of each team member's performance.
- **Aggregate Statistics**: Provides an overall summary of all the metrics for the entire team, offering a bird's-eye view of the team's collective performance.
- **Customizable Time Frame**: Users can set the time period for which the report is generated, making the tool flexible and adaptable to different project timelines.
- **Graphical Representation**: Visualizes the timeline data in the form of clear, intuitive graphs for easier comprehension and presentation.
- **Additional Metrics**: Apart from timeline analysis, this Action also reports on the number of open PRs, lines of code added or deleted, comments received on PRs, and the count of code reviews conducted by each developer. This comprehensive data set offers a deeper insight into the coding and collaboration activities of the team.
- **Developer and Team Overview**: While providing detailed data for individual developers, it also compiles an aggregate summary, enabling both micro and macro-level analysis of team performance.

This GitHub Action, **pr-full-report-action**, is an essential tool for any team seeking to optimize their software development process, ensuring more efficient and effective project management.

## Examples

## Configuration Parameters Overview

Below is a table outlining the various configuration parameters available for **pr-full-report-action**. These parameters allow you to customize the behavior of the action to fit your specific needs. Each parameter's name, description, requirement status, and default value (if applicable) are listed for your reference:

| Parameter Name           | Description                                                                      | Required | Default Value |
| ------------------------ | -------------------------------------------------------------------------------- | -------- | ------------- |
| `GITHUB_TOKEN`           | Github token                                                                     | Yes      | -             |
| `GITHUB_REPO`            | GitHub repository for report generation                                          | Yes      | -             |
| `GITHUB_OWNER`           | Owner of the GitHub repository                                                   | Yes      | -             |
| `GITHUB_REPO_FOR_ISSUE`  | GitHub repository for issue creation                                             | Yes      | -             |
| `GITHUB_OWNER_FOR_ISSUE` | Owner of the repository for issue                                                | Yes      | -             |
| `AMOUNT`                 | Number of pull requests in the report. Ignored if the `REPORT_DATE_START` is set | No       | `100`         |
| `REPORT_DATE_START`      | Start date for the report (d/MM/yyyy)                                            | No       | -             |
| `REPORT_DATE_END`        | End date for the report (d/MM/yyyy)                                              | No       | -             |
| `CORE_HOURS_START`       | Start of core hours (HH:mm)                                                      | No       | `10:00`       |
| `CORE_HOURS_END`         | End of core hours (HH:mm)                                                        | No       | `19:00`       |
| `PERCENTILE`             | Percentile value for timeline                                                    | No       | `75`          |
| `LABEL`                  | Label for the created issue                                                      | No       | -             |
| `ASSIGNEE`               | Assignee for the issue                                                           | No       | -             |

Use these parameters to tailor the **pr-full-report-action** to your project's specific requirements.

## Privacy and Data Handling

**pr-full-report-action** is designed with privacy and security in mind. It operates as a stateless application, ensuring it does not retain or store any user data externally. All processing is performed within your GitHub environment, maintaining strict data confidentiality. We prioritize the security of your information, ensuring no external data collection or storage, thereby safeguarding the integrity and privacy of your workflow.

## Usage Limitations

**pr-full-report-action** operates within GitHub's API rate limits and message size constraints, which are generally sufficient for detailed, long-term reporting. However, in rare cases of extremely large datasets, some adjustments might be necessary. For more information, refer to GitHub's documentation on [rate limiting](https://docs.github.com/en/rest/overview/rate-limits-for-the-rest-api). The length of the report generated by **pr-full-report-action** is limited to 65,536 characters due to GitHub Issue size constraints.

## Upcoming Features and Roadmap

At **pr-full-report-action**, we are committed to continuous improvement and adding functionalities that enhance your experience and the utility of our tool. Here's a glimpse into some exciting features and enhancements planned for the near future:

1. **Multi-Repository Reporting**: We are working on a feature that will allow users to compile reports across multiple repositories simultaneously. This will enable a more comprehensive analysis for teams managing multiple projects, providing a holistic view of their development activities.

2. **Detailed Open PR Discussions and Review Analysis**: Understanding the quality and depth of discussions in PRs is crucial. We plan to introduce more detailed reporting on open PR discussions and code reviews, offering insights into the nature and effectiveness of team collaborations and feedback.

3. **Enhanced Customization Options for Reports**: Recognizing the diverse needs of different teams, we aim to expand the customization capabilities of our reports. This enhancement will allow users to tailor reports more precisely to their specific requirements, ensuring that the reports are as relevant and informative as possible.

These upcoming features are designed with your feedback and needs in mind, striving to make **pr-full-report-action** more adaptable, insightful, and supportive of your project management and development workflows.

Stay tuned for these updates, and feel free to contribute your ideas or suggestions!

## License

**pr-full-report-action** is licensed under the [MIT License](https://opensource.org/licenses/MIT). This permits free use, modification, and distribution of the software, with the requirement of including the original copyright notice. For full license terms, see the [MIT License details](https://opensource.org/licenses/MIT).
