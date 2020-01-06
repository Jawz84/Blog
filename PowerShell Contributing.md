# Ten ways of contributing to PowerShell OSS

## Why this blog

I found [the documentation](https://github.com/PowerShell/PowerShell/blob/master/.github/CONTRIBUTING.md) on how to contribute to PowerShell/PowerShell a bit daunting.
The more links I followed, the more detailed and complex everything got.
At that point I felt I was not ready to contribute.
I did contribute anyway eventually.
And I realised there may be more people willing to contribute, but don't know where to start, and there does not seem to be a guide of how to start contributing to PowerShell in an easy way.
Also, there are ways to contribute apart from contributing C# code.

## How

You can contribute by lending your time and expertise.
There are so many ways to do so:
Blogging, speaking, teaching, sharing code, writing modules, or helping others on forums/channels (to name a few).
In this blog I want to focus on contributing to the PowerShell language directly.

## Where

There are a lot of repositories where you can contribute.
I choose to list these three, because here you can contribute to PowerShell itself most directly in my opinion:

- Documentation and Get-Help files: <https://github.com/MicrosoftDocs/PowerShell-Docs>
- Proposals about the language: <https://github.com/PowerShell/PowerShell-RFC>
- Engine & Language Issues, code and tests: <https://github.com/PowerShell/PowerShell>

## Why contribute

If you use PowerShell and you like it, chances are you have gained benefit from it.
Why not give back? You may learn a thing or two on the way, and the PowerShell OSS community is very helpful and friendly too.

If you would like a more thorough reasoning, I can recommend [Joel's blogpost on this](https://vexx32.github.io/2019/01/03/Contributing-Open-Source/).

## Ten ways to contribute

### 1. File a bug report

> Requires
> 
> - GitHub account

If you use PowerShell as your daily driver, or use it often on side projects, you may eventually run into something odd.

File that bug right here: <https://github.com/PowerShell/PowerShell/issues>

This is what you will be asked for when filing a bug:

- Make sure you are able to reproduce it on the [latest released version](https://github.com/PowerShell/PowerShell/releases)
- Search the [existing issues](https://github.com/PowerShell/PowerShell/issues)
- Refer to the [FAQ](https://github.com/PowerShell/PowerShell/blob/master/docs/FAQ.md)
- Refer to the [known issues](https://docs.microsoft.com/powershell/scripting/whats-new/known-issues-ps6?view=powershell-7)
- List steps to reproduce the bug
- Explain what you expected to happen
- Describe what actually happened instead
- Paste in relevant environment info: output of `$PSVersionTable` and if any, the error message

When in doubt, just share what you encountered to check if it's a bug in PowerShell or not.
Good places to share are:

- [Twitter](https://www.twitter.com), tag your tweet with #pshelp
- The [PowerShell Discord channel](https://aka.ms/psdiscord)\*
- The [PowerShell Slack channel](https://aka.ms/psslack)\*
- The [PowerShell IRC channel](https://poshcode.org/#irc)\*
- The [PowerShell/PowerShell Gitter channel](https://gitter.im/PowerShell/PowerShell)

\*) Discord, Slack and IRC are bridged via a channel called #Bridge. Read more about this on <poshcode.org>.

### 2. Help confirm bugs

> Requires
> 
> - GitHub account

Confirming bugs is going through recent bug report issues and trying to reproduce the bug.
This helps assess if a reported bug is really a bug or not.

A lot of new bug reports are going to have the ['Issue-Discussion'](https://github.com/PowerShell/PowerShell/issues?q=is%3Aissue+is%3Aopen+label%3AIssue-Discussion) label, instead of 'Issue-Bug'. 
This is because when you first open an issue on the PowerShell project, the automatic label for a bug report is Issue-Discussion, which typically won't be changed until a maintainer or collaborator has seen that the bug has been confirmed / reproduced by others or can reproduce it themselves.

You can comment in the issue whether or not you could repro it, and on which version of PowerShell.
Always try to reproduce a bug on the latest version of PowerShell.
Make sure you read the [FAQ](https://github.com/PowerShell/PowerShell/blob/master/docs/FAQ.md) and the [known issues](https://docs.microsoft.com/powershell/scripting/whats-new/).

If a bug is reproducible, it can be tested and fixed.
If a bug is not reproducible, more research may be needed.
You may be able to help the user who filed the bug with that.

> Tip: Consider 'Watching' the github repo.
You'll get a feel for what is going on daily.

### 3. Comment on language change proposals

> Requires
> 
> - GitHub account

The following things currently require an RFC:

- Large-scale changes to cmdlets
- **Any** changes to core language features
- New language features
- Deprecation of outdated features

Anyone can submit a proposal and  request comments from the community and the PowerShell Team.
Typically, an RFC will remain open for two months, to give everyone the opportunity to comment.
At this point, the PowerShell Committee will make the decision to approve or reject the RFC.

The RFC may also be discussed in the monthly call if there is reason to.

The full process is explained here: <https://github.com/PowerShell/powershell-rfc/blob/master/RFC0000-RFC-Process.md>

By commenting on an RFC, you can influence how an idea is going to be implemented, if at all.
Comments are valuable for the community and the committee to make a balanced decision, weighing all voices.

### 4. Attend the monthly PowerShell community call

> Requires
> 
> - A microphone and speakers
> - You can even join anonymously if you like 
> 
> Optional
> 
> - MS Teams
> - A headset
> - A camera

Every month, there is a call with PowerShell Team members and community members are invited! 
You can find the join link, as well as transcripts/youtube recordings of previous calls here: 
<https://github.com/PowerShell/PowerShell-RFC/tree/master/CommunityCall/>

Goal of the meeting is sharing roadmap/release info, and discussing RFC's.
You can join in, ask questions and let your voice be heard.
For example, if there is an RFC you have commented on, you can explain your view.

### 5. Suggest an improvement

> Requires
> 
> - GitHub account

You can also come up with ideas yourself!

If you have a cool improvement for a Cmdlet, a new feature or just a great idea, you can submit it as a [feature request](https://github.com/PowerShell/PowerShell/issues/new?assignees=&labels=Issue-Enhancement&template=Feature_Request.md&title=Feature+Request).

The maintainers will look at your idea and let you know what they think.
All genuine feature requests are handled with respect.
So don't be afraid to share your thoughts! 

Do take the time to find out if your idea has been proposed before and what was decided and why.
You can filter on the label 'Issue-Enhancement'.

In some cases it may be a good move to 'test' your idea against a few people first, before taking the time to fully explain what you have in mind in an issue, a great place to do so would be the [PowerShell Discord/Slack/IRC channel](https://poshcode.org).

### 6. Contribute Help content

> Requires
> 
> - GitHub account
> - Knowledge of Markdown
> 
> Optional
> 
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)

You can contribute by writing, improving, or expanding help files for Get-Help.
In particular, more examples for cmdlets are always welcome.

Head over to the <https://github.com/MicrosoftDocs/Powershell-Docs> repo, and read their [contributing manual](https://github.com/MicrosoftDocs/PowerShell-Docs/blob/staging/CONTRIBUTING.md) to get started.

> Tip: PowerShell Help is maintained for PowerShell versions 5.1 and higher. You may be asked to update help files for more than one version. 

To do small contributions like correcting typos, just navigate to that file, click the 'Edit' button, and GitHub will create a copy (fork) on your own GitHub for you.
When you are satisfied with your changes, you can save them, and submit a pull request to the _staging_ branch of the PowerShell-Docs repository.

For bigger contributions, you are better off cloning your fork locally to your computer.
This enables you to use VSCode and other editing tools.
A guide on how to do that can be found [here](https://github.com/MicrosoftDocs/PowerShell-Docs/blob/staging/contributing/1-GET-STARTED.md#making-major-edits-to-existing-topics).

With more examples, less typos, clearer wording, PowerShell can be easier to learn and use for everyone!

### 7. Write Pester tests

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Know how to run tests
> - Pester 4.8 or higher 
> - Pester knowledge 

Within the PowerShell project, many parts are tested automatically.
A big part of that is done with Pester.
See [here](https://github.com/PowerShell/PowerShell/tree/master/test/powershell).

> Tip: At the time of writing, Pester version 4.8.0 is used in the PowerShell project [`build.psm1` module](https://github.com/PowerShell/PowerShell/blob/a335063f1cb6596636031c2dc064fdf29924c5a7/build.psm1#L666).
This version pin will change in the future, as new versions of Pester become available.  

Many Cmdlets could use better or more extensive tests to verify they keep working correctly if someone changes them in the future.
So the Pester tests for CmdLets are kind of a safeguard against regression.
When there are more/better tests for CmdLets, you can possibly prevent future bugs!

See also [Details about contributing to the PowerShell/PowerShell repo](#Details-about-contributing-to-the-PowerShellPowerShell-repo), especially the section on how to run tests.

### 8. Write C# code for PowerShell

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Pester knowledge/know how to run test suite
> - An Integrated Development Environment that supports C#, like VSCode or Visual Studio
> - C# knowledge

When you solve an issue from the PowerShell/PowerShell repo by submitting code, you can make people's lives easier! 

Depending on your level of C# knowledge and experience, pick an issue that suits you, and let others know by commenting on the issue, that you would like to take it on.

> I picked a very small [issue](https://github.com/PowerShell/PowerShell/pull/9901), adding a `-Raw` switch to `Select-String`, because I did not know what to expect from the process, and from the code.
That worked well for me.

#### Editor

You can use VSCode with the [C# extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp), or you can use any version of Visual Studio.

#### Find code for a Cmdlet

There is a lot of code in PowerShell.
So where do you find the code you need to edit in order to solve the issue you picked? If you are are looking for the code for a specific Cmdlet, let's say `Get-Host`, you could search the codebase for 'Get-Host' and filter only \*.cs files, but you would not find it.
You will find if you search for 'Get, "Host' and filter \*.cs files only.
This is because Cmdlets names in C# are declared like this:

```C#
[Cmdlet(VerbsCommon.Get, "Host" /* abbreviated */ )]
```

#### Similarities between advanced functions and C# CmdLets

There are quite a few similarities between PowerShell advanced functions and how CmdLets need to be written in C#.
For example, the way parameters and parametersets are defined, and that there can be a `Begin`, `Process` and `End` block.

When you have C# experience, but have never written code for PowerShell, you should see the SDK reference [here](https://docs.microsoft.com/en-us/powershell/scripting/developer/Cmdlet/writing-a-windows-powershell-Cmdlet?view=powershell-7) to learn about concepts and find examples.

When you have little C# experience, but have written advanced PowerShell functions, you can still find your way.
When reading through the code, your starting point should be the `[Cmdlet()]` Attribute.
This is where parameters will be declared, just like in PowerShell.
And you will notice C# CmdLets have `BeginProcessing`, `ProcessRecord` and `EndProcessing` instead of the `Begin`, `Process` and `End` block.
After you have a little idea of what that looks like, find answers to questions that arise in the SDK linked above.

#### Finding your way in the code

If you are not super familiar with C# these tips may help you: 

- When you are working on a Cmdlet, you can set _breakpoints_ to be able to step through the code
- When you need information about where a certain method, property or variable comes from, use `F12` to [navigate to its definition](https://code.visualstudio.com/Docs/editor/editingevolved#_go-to-definition) 

> Tip: If you want to learn more about VSCode debugging for PowerShell, you can read more [here on the Microsoft scripting blog](https://devblogs.microsoft.com/scripting/debugging-powershell-script-in-visual-studio-code-part-1/), or watch [this video](https://youtu.be/cSbIXmlkr8o) from Tyler Leonhardt at PSconfEU 2019. The same principles work for the C# extension, as well as for Visual Studio.

See also [Details about contributing to the PowerShell/PowerShell repo](#Details-about-contributing-to-the-PowerShellPowerShell-repo).

### 9. Write C# xUnit tests

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Know how to run tests
> - Knowledge of the xUnit framework
> - C# knowledge

Only a small portion of all tests in the PowerShell/PowerShell repo are xUnit tests.
Most other tests are written in Pester.
Be sure to contact the PowerShell Team if you want to contribute here.
Most of the xUnit tests test internal PowerShell stuff.

The xUnit tests can be found here: 
<https://github.com/PowerShell/PowerShell/tree/master/test/xUnit>

If you want to use the tools from the `.\build.psm1` module, you may have to initialize a few options, like so:
`Get-PSOptions -DefaultToNew | Save-PSOptions` and then `Restore-PSOptions`.

If that is all set, you can start a test run for xUnit tests:

`Start-PSxUnit -xUnitTestResultsFile ".\<resultfilename>.xml"`

It will output to the file with the name you have specified to the folder `.\test\xUnit`, in xUnit format.

See also [Details about contributing to the PowerShell/PowerShell repo](#Details-about-contributing-to-the-PowerShellPowerShell-repo).

### 10. Write an RFC

> Requires
> 
> - GitHub account
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Firm understanding of PowerShell

Anyone in the community can write a proposal as a [Request For Comments](https://github.com/PowerShell/PowerShell-RFC) (RFC), and see what the committee and the community think.

If you have an idea that is bigger than just an Issue, you can consider writing a proposal. The first step to that is to file a feature request-type issue, so that the PowerShell Team can gauge whether there's interest in the requested change and there's an opportunity to hammer out a fairly well-rounded first draft.
This is because RFCs tend to be longer-form documents, and it can get rather lengthy to review them if changes constantly need to be hashed out during the review process.

Be sure to check the list of passed and rejected RFC's first.
You can read about the process [here](https://github.com/PowerShell/PowerShell-RFC/blob/master/RFC0000-RFC-Process.md).

Examples of past RFC's:

- Experimental-Accepted: [Abbreviation expansion based tab completion](https://github.com/PowerShell/PowerShell-RFC/blob/master/4-Experimental-Accepted/RFC0030-Abbreviation-Expansion-TabComplete.md)
- Experimental-Accepted: [ForEach-Object -Parallel Cmdlet](https://github.com/PowerShell/PowerShell-RFC/blob/master/4-Experimental-Accepted/RFC0044-ForEach-Parallel-Cmdlet.md)
- Final: [Obsoleting Send-MailMessage](https://github.com/PowerShell/PowerShell-RFC/blob/master/5-Final/RFC0042-Send-MailMessage.md)

RFC's are discussed at the monthly community call, and are open for comments for about two months, or longer as the committee sees fit.

> Tip: The Committee and the PowerShell Team members are separate; currently all Committee members are either current or past members of the PowerShell Team, but not everyone on the team is on the Committee. 
There is a desire to work out a process for adding community members to the Committee at some point in the future.

## Details about contributing to the PowerShell/PowerShell repo

### How to start

- Create an issue in the PowerShell repo, where you state that you would like to contribute Pester tests
- Ask the maintainers if there are any specific CmdLets that could use improved tests
- Fork the PowerShell repository to your own GitHub
- Clone your fork of the PowerShell repo to your local machine
- Create a new Git branch for your work

All Pester tests can be found in this folder:  
  `.\test\powershell`

Tests for built-in CmdLets are here:  
  `.\test\powershell\Modules`
  Especially the folders named `Microsoft.PowerShell.*`

Tests can also be found by using a search tool like VSCode's `Ctrl+F`. Just search for the Cmdlet you are looking for, and filter for filenames with `*.tests.ps1`

> Tip: If you forget to branch before you start working, `git stash; git stash branch newbranchname` is super super handy.
Also: <ohshitgit.com> for help after a git mishap.

### Alternative: develop within a container

VSCode has an extension for working in developement containers. 
The PowerShell repo supports that. 
If you use this, the repository will be opened in a Docker container on your system, and all necessary components will be inside the container. 
VSCode will connect to that container and you can work with it from there.

You will need:

- [Docker](https://www.docker.com/products/docker-desktop), configure a shared folder
- Give the Docker VM more RAM than just the default 2048MB if you can spare it, it will give you a nicer experience.
- VSCode [remote-development extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

Read more [here](https://code.visualstudio.com/docs/remote/remote-overview).

The first time, it will ask you to install recommended VSCode extensions, and loading the project may fail because of the missing extensions. 

- Install the recommended extensions and reload
- If VSCode tells you 'There are unresolved dependencies.' Click `Restore`

Now your environment should be all set.

- The terminal defaults to Bash. To start PowerShell, simply type `pwsh` 
- You can now load the `build.psm1` module with `Import-Module ./build.psm1` 
- In some cases you may need to run `Start-PSBuild -Clean`

### How to run a test

To run a test, you need to build the pwsh binaries first, and you need the test-tool.
Also note, if you run all tests, that's going to take some time.
Good thing there is an easy way!

In the base of the repository there is a module 'build.ps1', that has all kind of handy CmdLets in it for this kind of thing.
Load it like this:

`Import-Module .\build.psm1`

(If you want to know which tools are inside, use `Get-Command -Module build`)

The very fist time, you need to set up a few things.
To do that, run `Start-PsBootstrap` (may need sudo/adminstrative privileges, depending on your system.
On a docker container, it needs the `-NoSudo` switch).

You also need to build the pwsh binaries for the tests to run against: `Start-PsBuild`

> Tip: If you encounter weird build errors, just run `Start-PSBuild -Clean`.
This is generally a good idea every time you update your branch, or after a rebase.

Now you could simply run `Start-PSPester` to kick off a build, and run ALL Pester tests.
This would take some time, and this is still not what you want to do when writing extra tests, or improving existing ones.
So what do we do instead? We tell `Start-PSPester` which testfile we want to run:

`Start-PSPester -Path .\test\powershell\Modules\Microsoft.PowerShell.Core\Get-Command.Tests.ps1`

You will notice that it rebuilds test tool binaries each time you use Start-PSPester.
This takes time and usually we only need to build these binaries once.
To suppress new builds, you add the `-SkipTestToolBuild` switch:

`Start-PSPester -Path .\test\powershell\Modules\Microsoft.PowerShell.Core\Get-Command.Tests.ps1 -SkipTestToolBuild`

When writing and debugging your tests, remember that you can set breakpoints and step through your Pester code, this can help you find out where things are not going as they | Should -Be :-).

> Tip: If you want to learn more about VSCode debugging for PowerShell, you can read more [here on the Microsoft scripting blog](https://devblogs.microsoft.com/scripting/debugging-powershell-script-in-visual-studio-code-part-1/), or watch [this video](https://youtu.be/cSbIXmlkr8o) from Tyler Leonhardt at PSconfEU 2019.

For specific tips about how to use Pester within the PowerShell repo, be sure to read this document as an addendum to the Pester documentation: <https://github.com/PowerShell/PowerShell/blob/master/docs/testing-guidelines/WritingPesterTests.md>

### Updating your fork

So you have forked one of the GitHub repos, cloned it, tried stuff, but never created a PR. And now that fork is six months behind its ancester. How to update it? I'll describe how to do this for the PowerShell repo, this works the same for the other repos.

To update your GitHub fork, you will first update your local clone, and for that, you need to tell your local repository to which remote to look. 

- See which remotes are configured for your local repo: `git remote -v`
- If there is an entry with `https://github.com/PowerShell/PowerShell.git` in it, remember its name. It will usually be called 'upstream'
- If there is no entry present with that url, add it by typing:
`git remote add upstream https://github.com/PowerShell/PowerShell.git`
- Make sure there is an entry 'origin' with the url of your own GitHub url: `https://github.com/PowerShell/PowerShell.git` 

Make sure you have no uncommitted work on your branch. Stash or revert any uncommitted changes, and checkout to the master branch:

- To stash changes, go `git stash`
- To checkout master, do `git checkout master`

Now we need to check for changes and pull them in.

- Tell git to find out if there are changes in any of its remotes: `git fetch --all -p`
- Tell git to rebase your local repo on the 'upstream' remote (replace the name 'upstream' if necessary):
`git rebase upstream/master`

Rebasing is the way to tell git to replay your work on top of the other changes that were merged to master in the mean time. So now we have pulled in all changes from the original repo into our clone locally. These changes need to be pushed to your GitHub fork.

- Tell git to push local changes to origin: `git push` or `git push origin/master`.

For more detailed instructions with screenshots, see [here](https://info.sapien.com/index.php/version-control/github-how-to-update-your-fork).

### Submitting your contribution 

Do small git commits while you work, and don't forget to git push the work on your branch every once in a while.
When you are satisfied with your work, you can create a Pull Request.
You can create a PR from your own GitHub on the branch you created for you work on this.
It helps to reference your original Issue where you asked for guidance what to work on, use a '#' sign and put the number of your Issue behind it.
Fill any fields the PR requests from you.

Once you have created a PR, the automated CI process will start to run.
It will run ALL tests, on Windows, Linux and OSX.
You can follow the status of the running tests in your PR.
It takes around 20 minutes or so to finish.
Every time you push a new commit to your branch that you created the PR from, it will trigger a new CI run.

If you want to signal the maintainers that you are working on stuff, but are not ready yet, you can rename your PR to start with `WIP:` for Work In Progress.

Every Pull Request in the PowerShell repo gets an assignee.
A person who you can ask for help when something is not working properly (sometimes CI can be glitchy and fail on something else than your code), or if you just have a question.
Be patient - half of the work on the PowerShell repository is being done by volunteers, members of the community like you who do this in their spare time.
And staff members of the PowerShell Team have all kinds of tasks assigned to them.

Your work in the PR will be reviewed by two maintainers.
They will ask you to change things here and there, maybe even about code you did not touch, _because, just like you, they love PowerShell_ and they want the best for the product.
If you don't know what they mean, just say so, no worries.
They are all very helpful and friendly people.
It can take a few weeks for the whole review/finetuning process to complete.

Once all the CI checks turn green, and your reviewers are satisfied, your PR will be merged and your code is added to the codebase :-)

## Closing remarks

I hope this blog will help you find your way contributing to PowerShell. 
It's a great language, an even greater community. This offers all kinds of chances to learn new things, and meet new like minded people!
Please feel free to reach out to me if you have questions. 
You can [ping me on Twitter](https://www.twitter.com/Jawz_84), or drop me a message on Slack.

A special thank you goes to Joel (Sallow) Francis for reviewing!
