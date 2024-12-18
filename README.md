# 3DModel-Painter
## Purpose
This demo project was an experiment to explore the capabilities of the latest iteration of LLM-based code editors.
![3DModel Painter Screenshot](https://github.com/Xorlent/3DModel-Painter/blob/main/3DPainter.jpg)
## Background
_The entire codebase was powered by LLM generation only.  No fixes or other manual coding was performed to get this application to its current state._  
The coding workflow followed this basic pattern:
1. Create prompt to fully explain the features required for a minimally viable solution.
2. Review the generated code, update the prompt to better focus the LLM on the desired outcome.
3. Clear and repeat the prompt until a satisfactory code scaffold has been built.
4. Assess the code for errors or problematic behavior and ask the LLM to fix these areas of the application.
5. Continue to fine-tune the application until the desired outcome has been reached.
   - In my experience if you cannot resolve the issues within about 4 iterations, it is best to start over with a more concise or simplified prompt, as this is a good indication that the LLM does not fully understand how to generate the desired outcome.
## Operation
1. Download the .ZIP file
2. Extract the .ZIP file to the desired folder.  If you are on Windows, before extracting be sure to right-click the ZIP file, select "Properties" and click "Unblock."
3. Host the files using a local web server.
   - On Mac you can just open a terminal window, navigate to the 3D Model Painter folder and type:  
     ```python3 -m http.server 8080```
4. Open a web browser and navigate to the website.  Example:  http://localhost:8080/index.html
5. Click "Choose file" and select a GLTF 3D model file.
   - I included some 3D models you can play with in the /3dmodels folder.
7. Click and drag to rotate the model.
8. On the right, select a color or a texture map to begin painting faces of the model.  Once you have a color or texture map selected, click "Toggle Face Paint Mode"
   - When "Toggle Face Paint Mode" is red, you are painting
   - When "Toggle Face Paint Mode" is green, you can rotate the model
9. Texture map files can be any common image file format (PNG, JPG, SVG, WEBP), repeating patterns are best.
## Lessons Learned
1. It was relatively painless.  From start to finish I was able to generate this project in about 2 hours.
   - I estimate that learning three.js and coding this myself would have taken substantially longer, likely several days.
2. I think LLM-based code generation has now reached the point of being truly useful.  Some examples where I think it can be hugely helpful, especially to those of us that do not code for a living:
   - Refactoring spaghetti code.  I tend to start simple and iterate rapidly on all of my programming projects because I want working code in the shortest amount of time.  Maintainability is not high on my list of priorities; I want to implement my requirement and move on.  Is this painful later when implementing enhancements?  You bet!
   - Decomposing your project into very well-defined functions, classes, and methods, and asking the LLM to generate them individually.
   - Generating example code for APIs and libraries you need to learn.  I have found the example code to be far superior than what is found on the open web in programming forums.
   - Helping assess sections of code where a persistent bug could benefit from an independent review.
   - Improving error handling and helping to build test cases for existing code.
3. The most remarkable feature of LLM-based code editing is *actually helpful* code completion/recommendation.  This is a feature that was touted as a game-changer 10 years ago but more often than not, got in the way of a programmer's flow.  The current LLM code editor predition and recommendation accuracy capabilities are scary good!
