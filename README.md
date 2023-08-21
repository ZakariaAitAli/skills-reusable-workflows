<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses MIT license.
-->

# Reusable workflows and matrix strategies

_Make a workflow reusable, call it in another workflow, and use a matrix strategy to run multiple versions._

</header>

<!--
  <<< Author notes: Step 5 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 5: Trigger your workflow and view the Actions logs

_You're almost done. Last step! :heart:_

Now that the changes have been merged into the `main` branch, let's trigger the **My Starter Workflow** workflow to see everyting in action! But before we do, let's recall what we should expect to see before we run the workflow.

- We should expect to see five jobs running from our \*My Starter Workflow\*\*. Do you remember which ones? We have the `build` job and then the `call-reusable-workflow` job that has the matrix strategy.
  ![Screen Shot 2022-09-08 at 9 53 52 AM](https://user-images.githubusercontent.com/6351798/189220189-97361a5e-eecf-4666-a859-e0587354bafe.png)
- We should also expect to see the echo message printed as an output from the reusable workflow with the node version for each of the matrix version jobs.
  ![Screen Shot 2022-09-08 at 9 52 41 AM](https://user-images.githubusercontent.com/6351798/189220620-0576540a-366f-44e1-866c-2955af399cdb.png)

### :keyboard: Activity: Run the My Starter Workflow and view the Actions logs

1. Navigate to the **Actions** tab in your repo.
1. Choose the **My Starter Workflow** workflow from the left, and select the **Run workflow** button and run the workflow on the **Main** branch.
1. Wait a few seconds for the workflow run to appear in the queue. Once it shows, select the **My Starter Workflow** from the workflow runs queue.

Notice the list of build jobs on the left. One for the `build` job and four for the different node versions (14, 16, 18, 20) that you are running from your matrix. When one of the node version jobs complete, you can select that job and view the Actions logs for the **Output the input value**. This will print out the message from the reusable workflow file.

When you're done reviewing the Actions logs, return here and refresh the page to finish the course! 🎉

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/skills/.github/discussions) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
