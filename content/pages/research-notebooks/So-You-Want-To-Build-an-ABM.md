+++
title = "So you want to build an Agent-Based Model"
Description = ""
Tags = ["Notebooks"]
date = "2017-01-25"
draft=true

+++


Some consolidated thoughts from many conversations about building agent-based models:

- Be sure you *need* an ABM to answer the question you are asking
    - "ABMs are fun" isn't the best reason (although not the worst)

    
Major questions you'll need to answer for an economic ABM:

- Where does *behavior* come from? Be able to answer:
    - What is your agent's objective?
    - What are welfare costs of any approximate behavior?
    - What is the objective gradient around agents behavior? 
    - How to agents form expectations?
- Where do *prices* come from? 
    - This should follow fairly easily if you answer "behavior" well
- How do you *estimate / calibrate* your model?
    - Simulation-based estimation (MSM, SMLE) and DOE (Kriging metasimulation)


Toolkits, personal experience:

- Java: [Repast](https://repast.github.io/), [MASON](http://cs.gmu.edu/~eclab/projects/mason/): I have found these to almost always be overkill for my research work
- [Netlogo](https://ccl.northwestern.edu/netlogo/): great for fast prototyping, but poor optimization libraries (may have changed) and langauge is unpleasant
- Python: [Mesa](https://github.com/projectmesa/mesa) has made great progress lately
   - I usually program ABMs from scratch, but Mesa may woo me back to toolkits 


Resources:

[Leigh Tesfastsion: ACE](http://www2.econ.iastate.edu/tesfatsi/ace.htm)





