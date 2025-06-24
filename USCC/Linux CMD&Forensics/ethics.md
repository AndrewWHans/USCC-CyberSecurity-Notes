# Ethics in Linux Commmand Line & Forensics 🐧🚀🚀

1) Authorization is *EVERYTHING*
- **GOLDEN RULE**: Just because you can, doesn't mean you should.
- Having any analysis, scan, or command execution should be done **only** with explicit permission.
- Tools like nmap, tcpdump, dd, or bash scripts can expose or manipulate sensitive data.
> Example: don't run the sudo dd if=/dev/sda to clone a drive unless you are cleared for an incident response.

2) Integrity of Evidence
- In forensics, the ethical handling of evidence includes:
    1) Chain of Custody
    2) Write-blockers
    3) Verifiable hashes before and after acquisition

3) No Unauthorized Access
- Using your terminal to SSH, SCP, or brute force into machines you don't own or administer is **illegal and unethical**.
- Red teaming must be *contractual and scoped* via rules of engagement (ROE)

4) Data Privacy

5) Reporting over Retaliating
> ***To hack back or not*** relies on *heavily* understanding the particular conditions given, but a certain rule book:

    1) Hacking back is almost always unethical and illegal unless done under very specific, authorized conditions (e.g., government or law enforcement).
    2) Focus should be on evidence collection, containment, and reporting to authorities.


### References
[CloudFlare Blog: Trapping misbehaving bots in an AI Labyrinth](https://blog.cloudflare.com/ai-labyrinth/)
