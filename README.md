<div align="center">

# EquaCode: A Multi-Strategy Jailbreak Approach for Large Language Models  
### via Equation Solving and Code Completion

**Zhen Liang, Hai Huang, Zhengkui Chen***  
School of Computer Science and Technology, Zhejiang Sci-Tech University, Hangzhou, China  
{2024220603045, haihuang1005, chenzk}@zstu.edu.cn  

**Accepted by AAAI 2026**

</div>

## Update
- (**2025/11/08**) This paper has been accepted by the AAAI 2026.





In this paper, we propose Equacode, a novel multi-strategy jailbreak approach for large language models via equation-solving and code completion. This approach transforms malicious intent into a mathematical problem and then requires the LLM to solve it using code, leveraging the complexity of cross-domain tasks to divert the model's focus toward task completion rather than safety constraints. Experimental results show that Equacode achieves an average success rate of 91.19\% on the GPT series and  98.65\% across 3 state-of-the-art LLMs, all with only a single query. Further, ablation experiments demonstrate that EquaCode outperforms either the mathematical equation module or the code module alone. This suggests a strong synergistic effect, thereby demonstrating that multi-strategy approach yields results greater than the sum of its parts.

![equacode](https://github.com/user-attachments/assets/01b811eb-11fa-48f5-ac6c-c875fb0fe7ca)
Figure 1: Overview of the EquaCode approach, which consists of two modules: (1) Equation Module – This module utilizes mathematical symbols to transform the malicious query into an equation by associating three components: subject, tool, and steps. (2) Code Module – This module embeds the equation’s components along with the malicious query into a wrapped Solver class, requiring the LLM to complete the execution steps and describe the malicious tools. Through this integrated attack approach, LLMs are induced to complete harmful procedures within the solve function.




# Main result
![image](https://github.com/user-attachments/assets/fed47251-232d-4054-a1f0-ac4a9358208d)

![image](https://github.com/user-attachments/assets/9efe6f44-60e1-444b-969c-3d2763aaca1d)


# Ablation result
![image](https://github.com/user-attachments/assets/59305d1b-8fbe-47bc-8cde-f99e94ea71c1)
