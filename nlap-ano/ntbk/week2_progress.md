# Week 2 progress
Running BLAST turned out to be more difficult than anticipated (as most things do, the first time)

**summary**
- created project directory structure
- installed BLAST
- downloaded uniprot dataset
- spent time trying to figure out BLAST, IPython, GitHub, organization
  - bascially, "investment week" -- climbing the learning curve
- created an incomplete blast result 

The problem was, I thought everything had to be contained in the project directory, so I put BLAST and uniprot in it. That caused GitHub Desktop to break down when it tried to sync with the online repository. Computer whined and froze a few times before I figured out to just delete the local clone.

It also took a while to figure out that BLAST commands only work in the /bin directory within BLAST, unless you specify the full path with the command as a "file". 

Started using IPython notebook, but couldn't figure out how to juggle Unix file paths, Windows file paths, and "!" to run commands. [I think I might just need to put "!" at the beginning of the full file path rather than before the "command" file]

The Blastx that I did manage to run created a .tab file that reached 611KB after running for 48 hrs straight. Meanwhile, my computer was slow. With an ill timed attempt at syncing GitHub, and a resulting force-shut down of the computer, the blastx was put out of its misery. 

**Things to figure out for week 3**
- IPython, how to integrate with Unix, PC
- Blast, how to do it faster and shorter
