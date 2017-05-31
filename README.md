# playUserPassword

[![Build Status](https://travis-ci.org/mslinn/playUserPassword.svg?branch=master)](https://travis-ci.org/mslinn/playUserPassword)
[![GitHub version](https://badge.fury.io/gh/mslinn%2FplayUserPassword.svg)](https://badge.fury.io/gh/mslinn%playUserPassword)

User id/password authentication and authorization for Play 2.5.x projects, similar to the facilities provided by SecureSocial and Silhouette, but without any of the social authentication which complicates things.

### GitHub Pages
`sbtTemplate` sets up the GitHub pages branch for your new project.
Before you can use it, edit `build.sbt` and change this line so your GitHub user id and project name are substituted
for the placeholders `yourGithubId` and `my-new-project`:

    git.remoteRepo := "git@github.com:mslinn/play-user-password.git"


The Scaladoc for this project is [here](http://mslinn.github.io/play-user-password/latest/api/index.html)

#### Using sbtTemplate with Hub
Create a new SBT project and create a new GitHub project, which `hub` automatically adds as a `git` `remote`:

    $ sbtTemplate bigBadProject
    $ git create -d "Project description"
    two-factor authentication code: 881078
    Updating origin
    created repository: mslinn/bigBadProject

Now check in the new project:

    $ git add -A && git commit -m "Initial checkin" && git push -u origin master
