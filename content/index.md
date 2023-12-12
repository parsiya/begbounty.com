---
title: "Because You Gotta Beg for Disclosure!"
---

# Because You Gotta Beg for Disclosure!
My name is Parsia. I am an independent security engineer/researcher. This is
where I (hopefully) collect my disclosed security issues.

I am not a proper bug bounty hunter, I'd rather play videogames in my spare
time. Click on the link above to go to my personal website at
[parsiya.net](https://parsiya.net).

## Chaining Three Bugs to Get RCE in Microsoft AttackSurfaceAnalyzer
Write-up is at
https://parsiya.net/blog/2019-06-18-chaining-three-bugs-to-get-rce-in-microsoft-attacksurfaceanalyzer/.

Fix PRs:

* https://github.com/microsoft/AttackSurfaceAnalyzer/pull/218
* https://github.com/microsoft/AttackSurfaceAnalyzer/pull/220

## CVE-2020-13621 - Websites Can Run Arbitrary Code on Machines Running the 'PlayStation Now' Application - $15,000
Write-up is at https://hackerone.com/reports/873614. My first (and highest to
date) bounty.

Unfortunately, the images do not show up in the summary because the rest of the
report is not disclosed. However, the report goes through the whole discovery
process and should give you enough information to find your own bugs.

Note: The CVE is reserved but I never asked for assignment.

## CVE-2021-43907 - Remote Code Execution in Visual Studio Code's Remote WSL Extension
Yet another open local WebSocket server. Open a website while running VS Code in
WSL and get pwned!

The write-up has a lot of info about how VS Code server works which may help if
you want to hack it.

* Details:
  [https://parsiya.net/blog/2021-12-20-rce-in-visual-studio-codes-remote-wsl-for-fun-and-negative-profit/][code-wsl-rce].
* CVE page: [https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-43907][cve-2021-43907]

[code-wsl-rce]: https://parsiya.net/blog/2021-12-20-rce-in-visual-studio-codes-remote-wsl-for-fun-and-negative-profit/
[cve-2021-43907]: https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-43907