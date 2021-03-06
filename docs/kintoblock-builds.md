---
title: Git Repository, Builds & CI
---

## Continuous Integration and Deployment

When changes are committed into the repository branch, a new build for KintoBlock can be triggered by using the **Check for New Commits** button in the **KintoBlock Manage** page. Under **Recent Builds** user can view the recent commits made in the repository branch. The **Latest Build** section will be updated automatically with the last successful build.

The **Automatically build new commits in this branch** option automatically enables build generation for new commits in the repository. By default, the toggle switch is set to `ON`.


## Manually trigger builds for new Commits

To trigger a new build follow the steps mentioned below:

1. Open the KintoBlock.

2. Select the branch of KintoBlock consisting of the latest code.

3. Click on **Check for New Commits** button.

   { TODO: Raven Add GIF video of clicking on Check for New Commits button and new build generated }

A new build with last commits made in the repository will be generated. The status of the new build will be displayed in the **Recent Builds section**. If there are no new commits in the repository, a new build will not be generated.


## Re-generating builds via Retry

There is an option to regenerate a build from the last attempt to generated a build. Builds can be regenerated for all statuses: Success, Running and Failed.

To regenerate a build:

1. Open the KintoBlock build that resulted in failure.

2. Select the appropriate branch of the KintoBlock.

3. Click on the **Retry** button displayed in the build status table.

   { TODO: Raven Add a GIF video for clicking on Retry button and new build generated }

The build generation process will commence and the status of the build will be displayed in the **Recent Builds** section.


## View Repository

To view a repository, open any KintoBlock and scroll down to **Builds & Repository** section. The repository name of a KintoBlock is displayed right below the Recent Builds section under the title Repository.

The **Open Repo** button provides an option to quickly view the repository that is associated with your KintoBlock.
  
   { TODO: Raven Add image of Open Repo button }

The **View example projects link** in the Repository section provides an option to quickly view an example project of the programming language you have chosen to create the KintoBlock.


## View Build Logs

KintoHub maintains a structured list of the events that take place during the build generation. The entire build log can be generated in textual form by clicking on the **Open Log** button. 

   { TODO: Raven Add image of Open log button }

When the KintoBlock build is a success, you will notice a green banner on top of the Build Logs section with the title `No error found`.

If the KintoBlock builds results in failure, a red banner will be displayed on top of the Build Logs section with the title `Error found`.  Log messages can be analyzed to find the root causes of failure. 

   { TODO: Raven Add an image for error found }


## View Build Status

The Recent Builds section also displays the status of each build. The builds can have one of the 3 statuses mentioned below:

- **Running**: This is the initial state of a new build, while we build your KintoBlock

- **Success**: This status indicates that your KintoBlock build was run successfully.

- **Failure**: This status indicates that the build failed. 

Detailed logs pertaining to each status can be viewed by clicking on the status column.


## Tagging a Build

Builds are automatically generated when a KintoBlock is created. Tagging a build in a KintoBlock is a similar concept to tagging in GitHub. Once a build is tagged, the build can be referenced and deployed through a deployment. It’s important to tag stable builds that you have tested and prepared for production use!

To tag a commit in KintoBlock:

1. Open the KintoBlock you wish to tag.

2. Select the branch in your repository, where you have the final version of your KintoBlock that is ready to go!!

3. In **Builds & Repository section**, click on the **Tag Build** button for the commit that you would like to tag.

   { TODO: Raven Add image of Tag build button in Builds & Repository section }

4. Now specify the build number. We use the form  `MAJOR.MINOR.REVISION` for build numbers.

   { TODO: Raven Add GIF video of entering tag number }

5. Enter the release notes in the Notes section and then click on the **Tag Build**.

> Note: Tagging is important when you are preparing for public releases. If you want to update the deployment and add a KintoBlock to it, create a tag and select the tag within the deployment. This is an easy way to control the released versions of your KintoBlock.
