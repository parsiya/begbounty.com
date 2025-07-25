---
title: "Because You Gotta Beg for Disclosure!"
---

# Because You Gotta Beg for Disclosure!
My name is Parsia. I am a security engineer at Microsoft. This is where I
(hopefully) collect my disclosed security issues.

I am not a proper bug bounty hunter, I'd rather play videogames in my spare
time. Click the link above to go to my personal website at
[parsiya.net](https://parsiya.net).

## Chaining Three Bugs to Get RCE in Microsoft AttackSurfaceAnalyzer
Write-up is at [my blog][asa].
Fix PRs:

* https://github.com/microsoft/AttackSurfaceAnalyzer/pull/218
* https://github.com/microsoft/AttackSurfaceAnalyzer/pull/220

[asa]: https://parsiya.net/blog/2019-06-18-chaining-three-bugs-to-get-rce-in-microsoft-attacksurfaceanalyzer/

## CVE-2020-13621 - Websites Can Run Arbitrary Code on Machines Running the 'PlayStation Now' Application - $15,000
Write-up at https://hackerone.com/reports/873614. My first "real" bounty.

Unfortunately, the images do not show up in the summary because the rest of the
report is not disclosed. However, the report goes through the whole discovery
process and should give you enough information to find the same class of bugs.

Note: The CVE is reserved but I never asked for assignment.

Great explanation video by Bug Bounty Reports Explained YouTube channel: https://www.youtube.com/watch?v=97gPr9FdXzE

## CVE-2021-43907 - Remote Code Execution in Visual Studio Code's Remote WSL Extension
Yet another open local WebSocket server. Open a website while running VS Code in
WSL and get pwned!

The write-up has a lot of info about how VS Code server works which may help if
you want to do research there.

* Details:
  [https://parsiya.net/blog/2021-12-20-rce-in-visual-studio-codes-remote-wsl-for-fun-and-negative-profit/][code-wsl-rce].
* CVE page: [https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-43907][cve-2021-43907]
* I got to the front page of HackerNews, mom: https://news.ycombinator.com/item?id=29635300

[code-wsl-rce]: https://parsiya.net/blog/2021-12-20-rce-in-visual-studio-codes-remote-wsl-for-fun-and-negative-profit/
[cve-2021-43907]: https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-43907

## AWS Original Malicious Exploit or [AWSOME](/awsome.html)
It's a joke vulnerability. `Off-Off-Topic` is the everything goes chat channel
from the good ole' [Cigital][cigital]. We can squat S3 bucket names to prevent people from
deploying static websites.

In short, you need to own the bucket `apple.com` to deploy it as a static
website through S3. AWS bucket names are unique so you can hope someone else has
not created it.

~~I keep paying $15 a year for this domain because I like it.~~ It used to be
hosted at awsome[dot]pw, but I have stopped paying for the domain and moved the
page to this site at [/awsome.html](/awsome.html).

[cigital]: https://en.wikipedia.org/wiki/Cigital