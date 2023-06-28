# Approach #1 | Text-to-Text
    
The system will help users to generate text for one or multiple placeholders depending on the element context. 

| Technology readiness | Risks | Complexity |
| ----- | ----- | ---------- |
| 🟢 Ready for implementation | <div style="width: 100pt"> 🟡 Moderate risk | <div style="width: 150pt"> 🟢 Light complexity |


## Technologies

Open-source LLMs are already capable of working with this task, like open-llms [[Github](https://github.com/eugeneyan/open-llms)]. A solution like privateGPT [[Github](https://github.com/imartinez/privateGPT)] gives the ability to work offline with local files, increasing the security of the solution.

## Pipeline

Step #1) User selects elements or pages to populate with text
    
Step #2) System extracts information about the number and context of the module

Step #3) Based on input parameters, the Language model generates the output

Step #4) User verifies the output and approves the insertion
    

## Relevant works
Figma plugins presented here mostly demonstrate the possible interface of the implemented solution. 
    
- FigGPT [[Figma Plug-in](https://www.figma.com/community/plugin/1207913933994957698/FigGPT)] [[Website](https://www.olexdsgn.com/figgpt)]

- Cube GPT - UX AI Assistant [[Figma Plug-in](https://www.figma.com/community/plugin/1227828853742523809/Cube-GPT---UX-AI-Assistant)]

## Pros and Cons

🟢 Pros
    
- This approach would significantly streamline the process of generating text for placeholders, saving time and effort for designers.
- The system can adapt to different element contexts, ensuring the generated text is relevant and fits the design's purpose.
- With technologies like privateGPT, the system can work offline with local files, providing an added layer of data security.

🔴 Cons

- The success of this feature heavily relies on the system's ability to accurately determine the context of the module. That context should be pre-processed for the system, like count and type of placeholders, name, the functionality of the element, etc.
- AI can generate text based on context, but understanding the designer's precise intent or the emotion they wish to convey might be challenging. Especially in the visual domain.
