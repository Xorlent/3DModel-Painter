# 3DModel-Painter
## Purpose
This demo project was an experiment to explore the capabilities of the latest iteration of LLM-based code editors.
## Background
_The entire codebase was powered by LLM generation only.  No fixes or hand-coding was performed to get this application to its current state._  
The coding workflow followed this basic pattern:
1. Create prompt to fully explain the features required for a minimally viable solution.
2. Review the generated code, update the prompt to better focus the LLM on the desired outcome.
3. Clear and repeat the prompt until a satisfactory code scaffold has been built.
4. Assess the code for errors or problematic behavior and ask the LLM to fix these areas of the application.
5. Continue to fine-tune the application until the desired outcome has been reached.
   - In my experience if you cannot resolve the issues within about 4 iterations, it is best to start over, as this is a good indicator that the LLM does not fully understand how to generate the desired output.
## Operation
1. Download the .ZIP file
2. Extract the .ZIP file to a desired folder.  If you are on Windows, before extracting be sure to right-click the ZIP file, select "Properties" and click "Unblock."
3. Host the files using a local web server.
   - On Mac you can just open a terminal window, navigate to the 3D Model Painter folder and type:  
     ```python3 -m http.server 8080```
4. Open a web browser and navigate to the website.  Example:  http://localhost:8080/index.html
## Lessons Learned
1. From start to finish I was able to generate this project in about 2 hours.
  - I estimate that learning three.js and coding this myself would have taken substantially longer, likely several days.
2. I think LLM-based code generation has now reached the point of being truly useful.  Some examples where I think it can be hugely helpful, especially to those of us that do not code for a living:
    - 
3. The most remarkable feature of LLM-based code editing is *actually useful* code completion/recommendation.  This is a feature that was promised to be a game-changer 10 years ago but more often than not, got in the way of a programmer's flow.  The current LLM code editor predition and recommendation accuracy capabilities are scary good!
