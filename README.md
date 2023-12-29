# Leveraging software evolution data with LLMs
### JetBrains Internships Test task 

* Read [OctoPack: Instruction Tuning Code Large Language Models.](https://arxiv.org/pdf/2308.07124.pdf) 


* **Data exploration** ipynb file could be found [here](CommitPackFT_Data_Exploration.ipynb).

For the running just open it after the repository clone.

Other option is just open file in Colab using **Open in Colab** button (it could be found on top of the file in Preview)

Then run all cells. 

* The file with the evalution of HumanEvalPack could be found [here](Refact-1_6B-eval-final.ipynb). The running instruction 
is the same, but if you do not have GPU, follow the instruction in the notebook. 

Qualitative results are presented in the end of the notebook.

* This approach with using commits for code generating is already showing compelling results, by already outperforming
some other common code generating models. Hence, it could be really useful. However, observing HumanEvalPack Python dataset,
I have noticed that there are too low number of tasks in the dataset (for example, 'function misuse' is presented only by 8 task, what
says 0.25 performance in this case?). 

Additionally,  zero-shot pass metric is not presenting the performance well. My research for the thesis project now contains
the investigating RL algorithms in the NLP tasks. It could be more effective to take into the account the number of passed
unit tests, instead of yes/no answer for the whole group. 

To summarize, the commit usage for the code generating tasks could give even higher performance, and deserves to be considered as
a valid help.



