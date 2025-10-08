# ZeroDigyLab
An advanced AI powered analysis and suggestions tool. 

---

The system works in 2 modes: 

1. analysis
2. improovement



The analysis section is just recursive LLM calls with some other statistics, with the results saved to RESULT.json file. 

The analysis by the recursive LLM calls is based on wethods saved in METHODS.json .

The improovement mode is recursivly analysing the logs from the analysis mode, in order to create new, better methods, as well as update the effectiveness of methods. 