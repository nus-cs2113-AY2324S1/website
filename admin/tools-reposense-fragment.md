<pic src="https://reposense.org/images/reposenseOverview.png" />

We will be using a tool called [RepoSense](http://reposense.org) to make it **easier for you to see (and learn from) code written by others**, and to help us see who wrote which part of the code.

<pic src="https://reposense.org/images/report-features.png" alt="RepoSense report screenshot">
  <sub>Figure: RepoSense Report Features</sub>
</pic>

****Viewing the current status of code authorship data:****

* The reports generated by the tool for the individual and team projects will be made available in the course website at some point in the semester. The feature that is most relevant to you is the _Code Panel_ (shown on the right side of the screenshot above). It shows the code attributed to a given author.
* Click on your name to load the code attributed to you (based on Git blame/log data) onto the code panel on the right.
* If the code shown roughly matches the code you wrote, all is fine and there is nothing for you to do.

****If the code does not match the actual authorship:**** Given below are the possible reasons for the code shown to mismatch the code you wrote.
  * **Reason 1:** the `Author name` of some of your commits is not known to RepoSense -- this is a result of not setting the `git.username` property as instructed [in our Git setup instructions]({{ baseUrl }}/admin/tools.html#tool-git-for-revision-control).<br>
    **How to check:** Find the `Author name` of your commits that are _missing_ (you can use Sourcetree or the `git log` command for that -- it's not possible to do that using the GitHub interface though).<br> Check if that author name is included in the [RepoSense config for the iP](https://github.com/{{ course_org }}/ip-dashboard/blob/master/configs/author-config.csv) or the [RepoSense config for the tP](https://github.com/{{ course_org }}/tp-dashboard/blob/master/configs/author-config.csv) (whichever the applicable one)<br>
    **Remedy:** Send the missing author name(s) to the prof so that the RepoSense configuration can be updated accordingly.

  * **Reason 2:** The actual authorship does not match the authorship determined by git blame/log e.g., another student touched your code after you wrote it, and Git log attributed the code to that student instead.<br>
    **Remedy:** You can add `@@author` annotations as explained in the panel below:

<div class="indented-level2">
<panel header="Adding `@@author` tags to indicate authorship">
  <include src="reposenseAuthorAnnotation.md" />
</panel>
</div>

  * **Reason 3:** Some commits should not be included in the authorship analysis %%e.g., you committed the code of a third party library by mistake%%.<br>
    **Remedy:** Let us know the hashes of the commits that need to be omitted from the analysis.

If none of the above works, please please post in the [forum]({{ url_forum }}) or contact us via `{{ course | lower }}@comp.nus.edu.sg` so that we can advise you what to do.


==**We recommend you ensure your code is RepoSense-compatible by {{ version_penultimate }}**==