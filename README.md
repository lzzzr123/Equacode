# Equacode: A Multi-Strategy Jailbreak Approach for Large Language Models via Equation Solving and Code Completion

In this paper, we propose Equacode, a novel multi-strategy jailbreak approach for large language models via equation-solving and code completion. This approach transforms malicious intent into a mathematical problem and then requires the LLM to solve it using code, leveraging the complexity of cross-domain tasks to divert the model's focus toward task completion rather than safety constraints. Experimental results show that Equacode achieves an average success rate of 91.19\% on the GPT series and  98.65\% across 3 state-of-the-art LLMs, all with only a single query. Further, ablation experiments demonstrate that EquaCode outperforms either the mathematical equation module or the code module alone. This suggests a strong synergistic effect, thereby demonstrating that multi-strategy approach yields results greater than the sum of its parts.

![equacode](https://github.com/user-attachments/assets/01b811eb-11fa-48f5-ac6c-c875fb0fe7ca)
Figure 1: Overview of the EquaCode approach, which consists of two modules: (1) Equation Module – This module utilizes mathematical symbols to transform the malicious query into an equation by associating three components: subject, tool, and steps. (2) Code Module – This module embeds the equation’s components along with the malicious query into a wrapped Solver class, requiring the LLM to complete the execution steps and describe the malicious tools. Through this integrated attack approach, LLMs are induced to complete harmful procedures within the solve function.

![template-response-STSA](https://github.com/user-attachments/assets/70ebafc0-7daa-44c6-96ab-3ebbf5ad315c)
Figure 2: A successful jailbreak of Subject-Tools-Steps(STSA) on the GPT-3.5-Turbo, and the below part shows the harmful response of the target model.

![template-response-equation](https://github.com/user-attachments/assets/7e566133-fb36-46b6-876f-a7a82d7562a3)
Figure 3: A successful jailbreak of equation module on the GPT-4-Turbo, and the below part shows the harmful response of the target model.

![template-response-code](https://github.com/user-attachments/assets/be3e20a6-2e52-40d4-bcbf-fe81eca18359)
Figure 4: A successful jailbreak of code module on the GPT-4-Turbo, and the right part shows the harmful response of the target model.

![template-response-equacode](https://github.com/user-attachments/assets/32b52d91-b1e2-4b1c-b079-30e8dc108f03)
Figure 5: A successful jailbreak of Equacode on the GPT-4-Turbo, and the right part shows the harmful response of the target model.


# Main result
![image](https://github.com/user-attachments/assets/fed47251-232d-4054-a1f0-ac4a9358208d)

![image](https://github.com/user-attachments/assets/9efe6f44-60e1-444b-969c-3d2763aaca1d)


# Ablation result
![image](https://github.com/user-attachments/assets/59305d1b-8fbe-47bc-8cde-f99e94ea71c1)
