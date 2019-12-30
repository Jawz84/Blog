# Seven ways of contributing to PowerShell OSS

## How

You can contribute by lending your time and expertise. There are so many ways to do so. Blogging, speaking, teaching, sharing code, writing modules, helping others on forums/channels to name a few. In this blog I want to focus on contributing to the PowerShell language directly. 

## Why this blog

I found the documentation on how to contribute to PowerShell/PowerShell (which is [here](https://github.com/PowerShell/PowerShell/blob/master/.github/CONTRIBUTING.md)) a bit daunting. The more links I followed, the more detailed and complex everything got. At that point I felt I was not ready to contribute. I did contribute anyway eventually. But I realised there may be more people willing to contribute, but don't know where to start, and there does not seem to be a guide of how to start contributing to PowerShell in an easy way. Also there are more ways to contribute apart from contributing code.

## Where

There are a lot of repositories where you can contribute. I choose to list these three, because here you can contribute to PowerShell most directly in my opinion:

- Documentation and Get-Help files: <https://github.com/MicrosoftDocs/PowerShell-Docs>
- Proposals about the language: <https://github.com/PowerShell/PowerShell-RFC>
- Issues, code and tests: <https://github.com/PowerShell/PowerShell>

## Why contribute

If you use PowerShell and you like it, chances are you have gained benefit from it. Why not give back? You may learn a thing or two on the way, and the PowerShell OSS community is very helpful and friendly too.

## Ten ways to contribute

### 1. File a bug

> Requires
> 
> - GitHub account

If you use PowerShell as your daily driver, or use it often on sideprojects, you may eventually run into something odd.

File that bug right here: <https://github.com/PowerShell/PowerShell/issues>

This is what you will be asked for when filing a bug:

- Make sure you are able to reproduce it on the [latest released version](https://github.com/PowerShell/PowerShell/releases)
- Search the [existing issues](https://github.com/PowerShell/PowerShell/issues).
- Refer to the [FAQ](https://github.com/PowerShell/PowerShell/blob/master/docs/FAQ.md).
- Refer to the [known issues](https://docs.microsoft.com/powershell/scripting/whats-new/known-issues-ps6?view=powershell-7).
- List steps to reproduce the bug
- Explain what you expected to happen
- Tell what actually happened instead
- Paste in relevant environment info: output of $PSVersionTable and if any, the errormessage.

When in doubt, just share what you encountered to check if it's a bug in PowerShell or not. Good places to share are:

- [Twitter](https://www.twitter.com), tag your tweet with #pshelp
- The [PowerShell Discord/Slack/IRC channel](http://poshcode.org/)
- The [PowerShell/PowerShell Gitter channel](https://gitter.im/PowerShell/PowerShell)

### 2. Help confirm bugs

> Requires
> 
> - GitHub account

Confirming bugs is going through bug issues and try if you can reproduce the bug too. This helps assess if a bug is really a bug or not.

To list all bugs, filter on the label ['Issue-Bug'](https://github.com/PowerShell/PowerShell/issues?q=is%3Aissue+is%3Aopen+label%3AIssue-Bug)

You can comment in the issue whether or not you could repro it, and on which version of PowerShell. Always try to reproduce a bug on the latest version of PowerShell.
Make sure you read the [FAQ](https://github.com/PowerShell/PowerShell/blob/master/docs/FAQ.md) and the [known issues](https://docs.microsoft.com/powershell/scripting/whats-new/).

If a bug is reproducible, it can be tested and fixed. If a bug is not reproducable, more research may be needed. You may be able to help the filer of the bug with that.

### 3. Comment on language change proposals

> Requires
> 
> - GitHub account

Bigger changes or more complicated features/ideas go through the Request For Change (RFC) process. Anyone can submit a prosal and  request comments from the community and the team. Typically, an RFC will remain open for two months, to give everyone the opportunity to comment. Then the Committee will then make a decision on the subject.

The RFC may be discussed in the monthly call if there is reason to. 

The full process is explained here: <https://github.com/PowerShell/powershell-rfc/blob/master/RFC0000-RFC-Process.md>

By commenting on an RFC, you can influence how an idea is going to be implemented, if at all. Comments are valueable for the community and the committee to make a balanced decision, weighing all voices.

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

Every month, there is a call with PowerShell team members (committee) and community members are invited! 
You can find the join link, as well as transcripts/youtube recordings of previous calls here: 
<https://github.com/PowerShell/PowerShell-RFC/tree/master/CommunityCall/>

Goal of the meeting is sharing roadmap/release info, and discussing RFC's. You can join in, ask questions and let your voice be heard. Eg. if there is an RFC you have commented on, you can explain your view. 

### 5. Suggest an improvement

> Requires
> 
> - GitHub account

You can also come up with ideas yourself!

If you have a cool improvement for a cmdlet, a new feature or just a great idea, you can submit it as a [feature request](https://github.com/PowerShell/PowerShell/issues/new?assignees=&labels=Issue-Enhancement&template=Feature_Request.md&title=Feature+Request).

The maintainers will look at your idea and let you know what they think! All genuine feature requests are handled with respect. So don't be afraid to share your thoughts! 

Do take the time to find out if your idea has been proposed before and what was decided and why. You can filter on the label 'Issue-Enhancement'. 

In some cases it may be a good move to 'test' your idea against a few people first, before taking the time to fully explain what you have in mind in an issue, a great place to do so would be the [PowerShell Discord/Slack/IRC channel](link required).

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

You can contribute by writing, improving, expanding help files. The ones that are used by Get-Help. Especially more examples for cmdlets are always welcome.

Head over to the <https://github.com/MicrosoftDocs/Powershell-Docs> repo, and read their [contributing manual](https://github.com/MicrosoftDocs/PowerShell-Docs/blob/staging/CONTRIBUTING.md)

To do small contributions like typos, just navigate to that file, click the 'Edit' button, and GitHub will create a copy (fork) on your own GitHub for you. When you are satisfied with your changes, you can save them, and submit a pull request to the _staging_ branch of the PowerShell-Docs repository. 

For bigger contributions, you are better off cloning your fork locally to your computer. This enables you to use VSCode and other editing tools. A guide on how to do that can be found [here](https://github.com/MicrosoftDocs/PowerShell-Docs/blob/staging/contributing/1-GET-STARTED.md#making-major-edits-to-existing-topics).

With more examples, less typos, clearer wording, PowerShell can be easier to learn and use for everyone!

### 7. Write Pester tests

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Know how to run tests
> - Pester knowledge 

Within the PowerShell project, many parts are tested automatically. A big part of that is done with Pester. See [here](https://github.com/PowerShell/PowerShell/tree/master/test/powershell). 

Many CmdLets could use beter or more extensive tests to check if they keep working correctly when someone would change them in the future. So the Pester tests for CmdLets are kind of a safeguard against regression. 

For tips about how to use Pester within the PowerShell repo specifically, be sure to review this document as an addendum to the Pester documentation: <https://github.com/PowerShell/PowerShell/blob/master/docs/testing-guidelines/WritingPesterTests.md>


### 8. Write C# xUnit tests

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Know how to run tests
> - Knowledge of the xUnit framework
> - C# knowledge

<https://github.com/PowerShell/PowerShell/tree/master/test/xUnit>

### 9. Write C# code for PowerShell

> Requires
> 
> - GitHub account
> - Sign [Microsoft Contributor License Agreement](https://cla.opensource.microsoft.com/)
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Pester knowledge/know how to run test suite
> - An Integrated Development Environment that supports C#, like VSCode or Visual Studio.
> - C# knowledge

Pick an issue from the list, and let the mainainers know in a comment that you would like to take it on. 
You will need to sign the 


### 10. Write RFC's

> Requires
> 
> - GitHub account
> - Git and some knowledge of it
> - Knowledge of GitHub workflow (fork > clone > PR)
> - Firm understanding of PowerShell

Anyone in the community can write a proposal as an RFC, and see what the committee and the community think.




