For my project, I’d like to do a long-form blog post on the 2024 Crowdstrike outages- The source of the fault in the code, the method in which it was distributed, and how the way that something that Crowdstrike functions is something close to malware with trust. The idea of Kernel-level anticheat and cybersecurity software is becoming more and more prevalent, and it’s important to address the dangers inherent to such a thing.Since the first draft, I’ve found a few good sources to discuss, namely
https://learn.microsoft.com/en-us/troubleshoot/windows-server/setup-upgrade-and-drivers/support-policy-third-party-kernel-level-attestation
https://blogs.microsoft.com/blog/2024/07/20/helping-our-customers-through-the-crowdstrike-outage/
https://www.upi.com/Top_News/World-News/2024/07/19/IT-failure-hits-causes-chaos-around-world/2531721376791
https://techcommunity.microsoft.com/t5/intune-customer-success/new-recovery-tool-to-help-with-crowdstrike-issue-impacting/ba-p/4196959For the blog post itself, my current outline is something like this:

    Intro
        Summary of the incident (2024 software failure, crowdstrike software, kernel level)
            What is crowdstrike?

    What is a Kernel Level piece of software?
        Explain the different levels of an operating system
        Use Kernel Anticheat as an example
            Pieces of code tethered to the basic function of your computer, with full, unlimited access to work. Useful here to catch every process with unlimited discretion.
    How could faulty code distribute so quickly?
        Discuss the “backdoor” of automatic updates
        Explain why a piece of software like this needed it
            To keep up with new malware
        Ask if it really needed it.
    How did the failure work?
        Auto update with an out of bounds memory read - Bad kernel config would force a boot-loop and / or BSOD
            They pushed a fix, but this wasn’t installable when your computer was in a boot loop.
        Dangers of kernel-level software, accessing memory that didn’t exist.
    What were the consequences of this?
        911 Downtimes
        Airplanes grounded
        Massive disaster
        Inability to recover some systems.
            Needed to hard reset from an admin console, of which passwords might have been saved in the machine
    What’s changed since
        Very little.
        There were NO LEGAL CONSEQUENCES, just financial ones.
        Kernel level auto-updating software is a backdoor to your entire system. The entire aviation industry had a single point of failure.
    Conclusion
        Tech is so omnipresent in our society that it needs more and better legislation. Full stop, this should not be possible. This is something done unintentionally, and it’s harder to imagine more damage with a malicious attack, even.
