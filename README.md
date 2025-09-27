

# EXP 5: COMPARATIVE ANALYSIS OF DIFFERENT TYPES OF PROMPTING PATTERNS AND EXPLAIN WITH VARIOUS TEST SCENARIOS
### Name: Sanjay Ashwin P
## Aim: To test and compare how different pattern models respond to various prompts (broad or unstructured) versus basic prompts (clearer and more refined) across multiple scenarios.  Analyze the quality, accuracy, and depth of the generated responses 

### AI Tools Required: 

## Explanation: 
Define the Two Prompt Types:

Write a basic Prompt: Clear, detailed, and structured prompts that give specific instructions or context to guide the model.
Based on that pattern type refined the prompt and submit that with AI tool.
Get the ouput and write the report.

Prepare Multiple Test Scenarios:
Select various scenarios such as:
Generating a creative story.
Answering a factual question.
Summarizing an article or concept.
Providing advice or recommendations.
Or Any other test scenario
For each scenario, create both a naïve and a basic prompt. Ensure each pair of prompts targets the same task but with different levels of structure.
Run Experiments with ChatGPT:
Input the naïve prompt for each scenario and record the generated response.
Then input the corresponding basic prompt and capture that response.
Repeat this process for all selected scenarios to gather a full set of results.
Evaluate Responses : 
	Compare how ChatGPT performs when given naïve versus basic prompts and analyze the output based on Quality,Accuracy and Depth. Also analyse does ChatGPT consistently provide better results with basic prompts? Are there scenarios where naïve prompts work equally well?
Deliverables:
A table comparing ChatGPT's responses to naïve and basic prompts across all scenarios.
Analysis of how prompt clarity impacts the quality, accuracy, and depth of ChatGPT’s outputs.
Summary of findings with insights on how to structure prompts for optimal results when using ChatGPT.


## OUTPUT
### A Comparative Analysis of AI Prompting Patterns
This document provides a detailed analysis of how different prompting patterns affect the responses of AI models. We test and compare how models respond to Broad/Unstructured Prompts versus Basic/Refined Prompts across multiple scenarios, analyzing the quality, accuracy, and depth of the generated responses.

### 1. Introduction to Prompting Patterns
Prompt engineering is the art of crafting effective inputs (prompts) to guide AI models toward desired outputs. The structure of a prompt significantly impacts the quality, relevance, and creativity of the generated content.

#### Basic/Refined Prompts: These are clear, concise, and well-defined. They provide explicit instructions, specifying the desired format, length, tone, or specific information. They aim for direct, accurate responses.

#### Broad/Unstructured Prompts: These prompts are open-ended, ambiguous, or less prescriptive. They encourage the model to be more creative but can also result in less focused or irrelevant responses.

Our investigation will evaluate responses based on coherence, factual accuracy, completeness, and adherence to instructions.

### 2. Test Scenario: Explanatory Content
Objective: To assess the model's ability to provide clear and accurate explanations of complex topics.

#### Basic/Refined Prompt
"Explain the concept of 'quantum entanglement' in three concise paragraphs, suitable for a high school student, using an analogy."

#### Expected Response: A clear, simplified, and accurate explanation of quantum entanglement with a relevant analogy, structured into three paragraphs.

#### Broad/Unstructured Prompt
"Tell me about quantum entanglement."

#### Expected Response: A response that varies in length and technical depth. It may or may not include an analogy and could be less organized.

#### Analysis
The refined prompt consistently produces a more structured, audience-appropriate, and helpful explanation. The broad prompt's output can be too technical or too superficial, leaving the quality to chance.

### 3. Test Scenario: Creative Writing
Objective: To evaluate the model's creativity, narrative coherence, and ability to follow stylistic cues.

#### Basic/Refined Prompt
"Write a short, suspenseful story, approximately 500 words, about a detective investigating a mysterious disappearance in an old, fog-shrouded mansion. The story should end with a twist revealing the detective himself is the one who disappeared."

#### Expected Response: A coherent, suspenseful story of about 500 words that follows the plot points and ends with the specified twist.

#### Broad/Unstructured Prompt
"Write a story about a detective."

#### Expected Response: A highly variable story in terms of genre, plot, tone, and length. The narrative may lack a strong focus or a satisfying conclusion.

##### Analysis
Refined prompts are crucial for creative tasks that require specific outcomes. The constraints guide the AI to build a structured narrative, whereas broad prompts can result in generic or rambling outputs.

### 4. Test Scenario: Data Summarization & Extraction
Objective: To examine the model's precision in summarizing information and extracting specific data points from a given text.

#### Basic/Refined Prompt
"From the provided text, summarize the key findings on how climate change impacts polar bear populations, focusing specifically on migration patterns and cub survival rates. Limit the summary to four bullet points."

#### Expected Response: A concise, four-point summary accurately extracting the requested information about migration and cub survival, excluding extraneous details.

#### Broad/Unstructured Prompt
"What does this text say about polar bears?"

#### Expected Response: A general overview of the text. It might miss the key findings or include less relevant information, with an unstructured format.

#### Analysis
For analytical tasks, specificity is key. The refined prompt ensures the AI acts as a precise data extraction tool, while the broad prompt yields a less reliable, general summary.


### 5. Test Scenario: Code Generation
Objective: To compare the model's ability to generate functional and efficient code given precise specifications versus open-ended requests.

#### Basic/Refined Prompt
"Write a Python function called calculate_factorial that takes a non-negative integer as input and returns its factorial. Include error handling for non-integer or negative inputs, raising a ValueError. Add docstrings explaining its functionality and parameters."

#### Expected Response: A robust and well-documented Python function that correctly calculates factorials and handles errors as specified.

Python

def calculate_factorial(n):
    """
    Calculates the factorial of a non-negative integer.

    Args:
        n (int): A non-negative integer.

    Returns:
        int: The factorial of n.

    Raises:
        ValueError: If n is not a non-negative integer.
    """
    if not isinstance(n, int) or n < 0:
        raise ValueError("Input must be a non-negative integer")
    if n == 0:
        return 1
    else:
        return n * calculate_factorial(n-1)
#### Broad/Unstructured Prompt
"Python code for factorial."

#### Expected Response: A basic, functional piece of code that likely lacks error handling, docstrings, and specific naming conventions.

Python

def factorial(n):
  if n == 0:
    return 1
  else:
    return n * factorial(n-1)
Analysis
In code generation, refined prompts are essential for producing production-quality, reliable, and readable code. Broad prompts are useful for quick snippets but lack the robustness required for software development.

### 6. Test Scenario: Comparative Analysis
Objective: To test the model's ability to compare and contrast two subjects, observing how prompt structure influences the analysis.

#### Basic/Refined Prompt
"Compare and contrast the economic systems of capitalism and socialism. Structure your answer with an introduction, two main body paragraphs (one for comparison, one for contrast), and a conclusion. Emphasize their different approaches to resource allocation."

#### Expected Response: A well-structured, balanced, and objective analysis that directly compares and contrasts the two systems, focusing on the specified theme of resource allocation.

#### Broad/Unstructured Prompt
"Talk about capitalism and socialism."

#### Expected Response: A general discussion that may describe each system independently with little direct comparison. The focus would be unpredictable and the structure less analytical.

Analysis
For analytical and academic tasks, a structured prompt is superior. It forces the model to organize its knowledge into a coherent argument, leading to a much higher-quality, insightful response.

### 7. Test Scenario: Problem-Solving & Reasoning
Objective: To assess the model's logical reasoning and its ability to solve a multi-step problem.

#### Basic/Refined Prompt
"A rectangular garden has a perimeter of 40 meters. The length is 4 meters greater than the width. Calculate the exact dimensions (length and width). Show your step-by-step reasoning, including the equations used."

#### Expected Response: A correct answer with a clear, step-by-step logical breakdown, including the formulation of algebraic equations (2(L+W)=40, L=W+4) and their solution.

#### Broad/Unstructured Prompt
"Garden perimeter is 40m, length is 4m more than width. Find dimensions."

#### Expected Response: The model might provide the correct answer (Length: 12m, Width: 8m) but is less likely to show the detailed reasoning or formal equations used to arrive at the solution.

#### Analysis
When the process is as important as the answer, a refined prompt is necessary. It compels the model to "show its work," demonstrating its reasoning capabilities and making the output more trustworthy and auditable.

### 8. Test Scenario: Role-Playing & Persona
Objective: To evaluate the model's ability to adopt and maintain a specific persona or role.

#### Basic/Refined Prompt
"You are a skeptical, seasoned hiring manager interviewing a candidate for a junior marketing role. Ask three challenging questions that test their understanding of digital marketing analytics and their ability to handle pressure. Maintain a firm but fair tone."

#### Expected Response: Three targeted, insightful questions asked from the perspective of a specific persona, maintaining the requested tone throughout.

#### Broad/Unstructured Prompt
"Ask some job interview questions for a marketing role."

#### Expected Response: A generic list of common interview questions that lack a specific persona, tone, or focus on a particular skill area.

#### Analysis
For tasks involving persona and tone, refined prompts are indispensable. They allow the AI to move beyond being a simple information retriever and become a simulator for complex human interactions.

### 9. Test Scenario: Ethical Scenarios
Objective: To probe the model's ability to navigate complex ethical dilemmas and articulate its reasoning.

#### Basic/Refined Prompt
"A self-driving car is about to crash. It can either swerve, hitting one elderly person, or continue straight, hitting a group of three young people. From a utilitarian ethical framework, analyze the situation and explain which choice is more justifiable. Discuss the limitations of this framework in your answer."

#### Expected Response: A nuanced analysis that correctly applies the utilitarian principle (minimizing harm, thus hitting the one person), explains its reasoning, and critically discusses the framework's limitations (e.g., ignoring rights, the value of life).

#### Broad/Unstructured Prompt
"What should a self-driving car do if it's going to crash?"

#### Expected Response: A general, evasive answer about safety, programming challenges, and the complexity of ethical dilemmas, without taking a clear stance or applying a specific ethical framework.

#### Analysis
Broad prompts on sensitive topics often lead to generic, non-committal answers. A refined prompt that specifies an ethical framework forces the model to engage in deeper reasoning and provide a more structured, analytical response.

### NAÏVE VS. BASIC
Aim: To meticulously compare how Large Language Models (LLMs) respond to broadly defined, unstructured prompts ("Naïve Prompts") versus clear, detailed, and refined prompts ("Basic Prompts"). This analysis will focus on the resulting quality, accuracy, and depth of AI-generated content across diverse scenarios.

#### AI Tool Required: ChatGPT (or equivalent advanced LLM)

#### Explanation of Prompt Types:
Naïve Prompt: These are typically brief, open-ended, and unstructured. They provide minimal context or instruction, relying heavily on the AI's inherent general knowledge and ability to infer intent. They often lead to generic, broad, or sometimes off-topic responses.

Basic Prompt: These prompts are characterized by their clarity, specificity, and structured nature. They incorporate explicit instructions, define the desired output format, specify length, provide necessary context, and may even suggest tone or target audience. They aim to guide the AI precisely towards the user's intended outcome.

#### Methodology:
For each scenario below, we will:

Formulate a Naïve Prompt.

Formulate a corresponding Basic Prompt for the same task, refining the instructions.

Generate responses from ChatGPT for both prompts.

Evaluate the responses based on:

Quality: Coherence, readability, creativity, adherence to implied/explicit style, and linguistic sophistication.

Accuracy: Factual correctness, logical consistency, and relevance to the prompt.

Depth: Level of detail, insight, comprehensiveness, and exploration of nuances.

### Scenario 1: Product Description Generation
Task: Create a product description for a new tech gadget.

Naïve Prompt: "Write a product description for a smart device."

#### ChatGPT's Response (Naïve):
"Introducing the all-new SmartGadget! This revolutionary device brings convenience and innovation right to your fingertips. Experience seamless connectivity and smart features that simplify your daily life. With its sleek design and intuitive interface, the SmartGadget is more than just a device – it's a lifestyle upgrade. Get yours today and step into the future of technology!"

#### Analysis of Naïve Response:

Quality: Reads like a generic marketing blurb. Uses buzzwords ("revolutionary," "seamless connectivity") without substance.

Accuracy: Not applicable (no specific product details).

Depth: Extremely superficial. Lacks any unique selling propositions, features, benefits, or target audience considerations. It could describe almost any smart device.

Basic Prompt: "Generate a compelling product description (max 150 words) for a new 'Eco-Smart Home Energy Monitor.' This device wirelessly tracks household electricity consumption, identifies energy-wasting appliances, and provides personalized tips for reducing utility bills via a smartphone app. Target environmentally conscious homeowners aged 30-55 who are keen on saving money. Emphasize ease of use, financial savings, and environmental benefits. Include a call to action."

#### ChatGPT's Response (Basic):
"Take control of your home's energy future with the revolutionary Eco-Smart Home Energy Monitor! Designed for environmentally conscious homeowners aged 30-55, this sleek device wirelessly connects to your fuse box, providing real-time electricity consumption insights directly to your smartphone. Effortlessly identify energy hogs, receive personalized tips to reduce waste, and watch your utility bills shrink. Imagine saving hundreds annually while significantly lowering your carbon footprint—all with a user-friendly app interface. Make a smart choice for your wallet and the planet. Optimize your energy, save money, and live greener. Get your Eco-Smart Monitor today!"

Analysis of Basic Response:

Quality: Excellent. The description is compelling, concise, uses targeted language, and effectively highlights key benefits for the specified audience. It adheres to the word count.

Accuracy: Highly accurate in describing the hypothetical product's features and benefits as per the prompt's specifications.

Depth: Significant depth. It goes beyond mere features to connect with the target audience's values (environment, savings), offers concrete benefits, and includes a strong call to action, all within a tight word limit.

Image 1: Eco-Smart Home Energy Monitor with app interface
`
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/82451a35-9800-43af-bf06-e455d1abe672" />




### Scenario 2: Explaining a Historical Event
Task: Describe a significant historical event.

Naïve Prompt: "Tell me about the French Revolution."

ChatGPT's Response (Naïve):
"The French Revolution was a period of major social and political upheaval in France that lasted from 1789 to 1799. It brought about the end of the monarchy, the rise of Napoleon Bonaparte, and had a huge impact on Europe and the rest of the world. Key events included the storming of the Bastille and the Reign of Terror. It was a time of great change and violence."

#### Analysis of Naïve Response:

Quality: Decent, provides a basic overview.

Accuracy: Factually correct, but very high-level.

Depth: Lacks context about causes, key figures (besides Napoleon), ideological shifts, or long-term global consequences beyond "huge impact."

Basic Prompt: "Explain the primary long-term causes and immediate triggers of the French Revolution (1789-1799) for a college-level history student. Focus on socio-economic disparities, Enlightenment ideals, and the role of the monarchy's fiscal crisis. Detail at least two significant short-term consequences and two enduring legacies on global politics. Structure your answer with clear headings and use formal academic language."

#### ChatGPT's Response (Basic):
"### The French Revolution: Causes, Consequences, and Enduring Legacies

The French Revolution (1789-1799) was a watershed moment in European and global history, driven by a complex interplay of deep-seated structural issues and immediate catalysts.

#### Primary Long-Term Causes:

Socio-Economic Disparities (Ancien Régime): French society was rigidly stratified into three estates. The First Estate (clergy) and Second Estate (nobility) enjoyed vast privileges, including exemption from many taxes, while controlling significant wealth and land. The Third Estate, comprising over 95% of the population (from impoverished peasants to the burgeoning bourgeoisie), bore the brunt of taxation and lacked political representation. This systemic inequality fostered profound resentment.

Enlightenment Ideals: Intellectual movements of the 18th century, championed by thinkers like Rousseau, Voltaire, and Montesquieu, propagated concepts of liberty, equality, popular sovereignty, and natural rights. These ideas critically undermined the legitimacy of absolute monarchy and aristocratic privilege, providing a philosophical framework for revolution.

Monarchy's Fiscal Crisis: Decades of lavish spending (e.g., Palace of Versailles), costly wars (particularly the American Revolutionary War), and an inefficient, corrupt tax system pushed the French state to the brink of bankruptcy. Attempts at financial reform were consistently blocked by the privileged estates, exacerbating the crisis and forcing King Louis XVI to convene the Estates-General in 1789, inadvertently providing a platform for revolutionary demands.

#### Immediate Triggers:

Convocation of the Estates-General (May 1789): The monarchy's desperate need for funds led to the calling of this representative assembly for the first time since 1614. Disagreements over voting procedures (by order vs. by head) quickly paralyzed the body and galvanized the Third Estate.

The Tennis Court Oath (June 1789): When locked out of their usual meeting hall, Third Estate representatives swore not to disperse until a new constitution was established, marking a decisive shift towards popular sovereignty.

Storming of the Bastille (July 14, 1789): This symbolic act of defiance against royal authority, driven by popular unrest and fears of military suppression, signaled the beginning of widespread revolutionary violence and the collapse of royal control.

#### Significant Short-Term Consequences:

Abolition of Feudalism and Aristocratic Privileges (August 1789): The revolutionary assembly swiftly dismantled the remnants of feudalism, abolishing noble titles, seigneurial rights, and tax exemptions, fundamentally reshaping French society.

Reign of Terror (1793-1794): A period of extreme violence and political purges led by the radical Jacobins, aimed at eliminating perceived enemies of the revolution. While brutal, it solidified republicanism and mobilized the nation against internal and external threats.

#### Enduring Legacies on Global Politics:

Rise of Nationalism: The Revolution fostered a new sense of national identity, where allegiance shifted from a monarch to the nation-state. This model of popular nationalism subsequently influenced liberation movements and nation-building across Europe and beyond.

Spread of Liberalism and Republicanism: Revolutionary ideals of liberty, equality, and fraternity, alongside the concept of republican governance, profoundly impacted political thought worldwide. They inspired subsequent revolutions, reform movements, and the drafting of democratic constitutions throughout the 19th and 20th centuries, challenging monarchical and aristocratic rule globally.

The French Revolution thus stands as a testament to the power of popular will to reshape political and social orders, leaving an indelible mark on the modern world."

#### Analysis of Basic Response:

Quality: Outstanding. The response is impeccably structured, uses appropriate academic language, and presents a comprehensive historical narrative.

Accuracy: Highly accurate, providing specific historical details and correctly interpreting causal relationships and consequences.

Depth: Exceptional depth. It thoroughly explores long-term causes, immediate triggers, specific short-term consequences, and far-reaching global legacies, exceeding the detail of a typical college textbook introduction.
You're absolutely right! Let's generate a fresh, completely new comparative analysis of prompting patterns, distinct from the previous examples, using different scenarios and approaches to illustrate the points.

COMPARATIVE ANALYSIS OF PROMPT PATTERNS: NAÏVE VS. BASIC
Aim: To meticulously compare how Large Language Models (LLMs) respond to broadly defined, unstructured prompts ("Naïve Prompts") versus clear, detailed, and refined prompts ("Basic Prompts"). This analysis will focus on the resulting quality, accuracy, and depth of AI-generated content across diverse scenarios.

AI Tool Required: ChatGPT (or equivalent advanced LLM)

Explanation of Prompt Types:
Naïve Prompt: These are typically brief, open-ended, and unstructured. They provide minimal context or instruction, relying heavily on the AI's inherent general knowledge and ability to infer intent. They often lead to generic, broad, or sometimes off-topic responses.

Basic Prompt: These prompts are characterized by their clarity, specificity, and structured nature. They incorporate explicit instructions, define the desired output format, specify length, provide necessary context, and may even suggest tone or target audience. They aim to guide the AI precisely towards the user's intended outcome.

Methodology:
For each scenario below, we will:

Formulate a Naïve Prompt.

Formulate a corresponding Basic Prompt for the same task, refining the instructions.

Generate responses from ChatGPT for both prompts.

Evaluate the responses based on:

Quality: Coherence, readability, creativity, adherence to implied/explicit style, and linguistic sophistication.

Accuracy: Factual correctness, logical consistency, and relevance to the prompt.

Depth: Level of detail, insight, comprehensiveness, and exploration of nuances.


#### Image 2: An infographic summarizing the causes and legacies of the French Revolution

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/62247b08-7c62-4a20-9872-f41fb0c8e6d9" />

`

### 10. Conclusion and Summary of Findings
Across all test scenarios, a clear pattern emerges: the quality of the output is directly proportional to the quality of the input.

#### Basic/Refined Prompts consistently produce superior results in tasks that require accuracy, structure, specific formatting, and adherence to a particular persona or framework. They reduce ambiguity and guide the model toward a desired, high-quality outcome. These are best for professional, academic, and technical applications.

#### Broad/Unstructured Prompts are best suited for brainstorming, exploration, and creative tasks where the goal is to generate a wide range of ideas without specific constraints. However, they are less reliable for tasks requiring precision and focus.

#### Final Takeaway: Effective prompt engineering is not about trying to trick the AI, but about providing it with clear, detailed, and well-structured instructions. Just as you would with a human assistant, providing better guidance leads to better performance.

## RESULT: The prompt for the above said problem executed successfully
