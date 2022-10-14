# UC-DTR

The UC-DTR algorithm exploits causal bounds to provide provably tighter estimates of the value of policies in a dynamic
treatment regime (DTR), a kind of non-Markovian decision process studied in medical literature on multi-stage clinical interventions.  I investigated this algorithm due to an interest in whether it could be used for machine translation in low-resource settings involving artificial languages with unidirectional semantics.  In the process, I reimplemented the UC-DTR algorithm presented in [UC-DTR](https://papers.nips.cc/paper/2019/hash/8252831b9fce7a49421e622c14ce0f65-Abstract.html) paper (Zhang & Bareinboim, 2019).  I am grateful to the original authors, who were kind to share their original implementation with me privately.

Install the requirements specified by `requirements.txt` and run the standalone script with `python uc_dtr.py [--help]`.  The default parameters allow the script to run at a tolerable speed on my local machine.  Upon completion, a plot of the rolling average regret resulting from random exploration and UC-DTR is saved to `uc_dtr_simulation-TIMESTAMP.png`.
