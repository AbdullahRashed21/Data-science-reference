# Classification Course Project Success Guide

Metis projects are graded by point assignments for five component parts, each on a scale of 1 to 5. A score of 3 on a 
component indicates that the project requirements for that component have been well met, while scores below and above 3 
respectively indicate that requirements are not met or are significantly exceeded. The components are: **design**, **data**, 
**algorithms**, **tools**, and **communication**. A total score of 15 (average of 3 per component) is required to successfully 
pass the course.

For specific instructions on this project's requirements, refer to the [project introduction](./project_intro.md). 
Below are guidelines mapping out the typical project factors in each component that lead to a score of 3, as well as 
those that help contribute to being below or above a 3. 
**Note that these factors are guidelines and are not prescriptive**; instructors will ultimately grade based on their 
careful judgement in conjunction with these guidelines, 
so it is not a good idea to try to "game" these guidelines. 

If in doubt about expectations or a score received, you may always consult the instructional team.

**Important note on deliverable deadlines**: Refer to the [daily schedule](../../README.md) for all project deliverables and their deadlines, both intermediate (project proposal, MVP) and final (slides, writeup and code). If you submit your final deliverable later than 11 am ET on presentation day, you will receive a 1 point penalty under the Design category. If you don't submit by 3 pm ET on that day, **we will not be able to grade your project and you will not pass the course**. Any exceptional circumstances should be discussed with your instructors and program manager as soon as possible. You should also meet the intermediate deliverable deadlines  -- your ability to keep to deadlines and display professionalism in your project work will be scored under the design category.

### Design:

*  **Satisfactory**: Includes a properly framed, useful classification problem addressable with selected data. All 
deliverable deadlines are met.  

*  **Below**: Project choice is not appropriate for classification methods, deliverable deadlines are not met.
*  **Above**: Demonstrates exceptional creativity and proficiency in leveraging classification techniques to address a 
complex, useful question. 

### Data:

*  **Satisfactory**: Primary data includes either 10,000+ data points and 10+ features, or 
sufficient complexity for interesting modeling challenges (consult with an instructor if in doubt).

*  **Below**: Data set is small or overly simple. 
*  **Above**: Data is large in scale, both in data points (~1,000,000+) and features.
Data has significant formatting/handling complexities such as requiring extensive preprocessing or having an unusual 
structure (e.g. geographic or hierarchical data). 
Multiple datasets are leveraged via merging disparate sources.  
 
### Algorithms

Note that students **are not graded based on evaluation metric scores**: we are looking for soundness in approach and 
rigor in exploring the problem you've chosen as thoroughly as possible. Classification problems will vary widely in the 
predictive challenge they pose, and the "success" of a model is contextualized by this level of challenge, not by absolute 
metric numbers. 

*  **Satisfactory**: A classification model is successfully built and tuned using a rigorous selection/evaluation 
framework (i.e. with proper validation and testing and a reasonable choice of metric). Regularization, feature engineering, 
ensembling, and class imbalance techniques are applied as appropriate, and model results are interpreted correctly. 

*  **Below**: No classification model is built, the model outputs are interpreted incorrectly, or the model built is 
deficient in approach -- e.g., the model is evaluated only on training data or has a glaring overfitting problem that 
could be addressed with regularization.      
*  **Above**: A carefully curated classification model is built: rigorous feature selection and engineering is performed, 
with the model's end application always clearly in mind. Meticulous attention is paid to model selection methodology, 
to the point of considering model scalability and complexity/interpretation tradeoffs. Models are used and analyzed with 
finesse to gain insight into complex interpretation problems. Models beyond the scope of the course are built, their use 
understood and well-justified by the student.  

### Tools

*  **Satisfactory**: At least one Python package for classification is used correctly and effectively to build 
classification models. 

*  **Below**: Python packages for classification are not used, or are used trivially or incorrectly.

*  **Above**: Python packages for classification are used to an advanced degree, beyond what was covered in the course. 
Significant data/engineering tools not covered in the course are used.

- Major examples of applicable tools not covered in the course:
  - *Acquisition* tools could include web scraping libraries or use of APIs  
  - *Storage* tools could include SQL or noSQL (e.g. MongoDB) databases
  - *Processing* tools could include Google Cloud or Amazon Web Services for cloud computing resources
  - *Visualization* tools could include Python libraries such as Bokeh and Plotly or resources outside of Python such as Tableau
  - *Production* tools could include Flask or other web app libraries/technologies



### Communication:
 
*  **Satisfactory**: Presentation is in line with time requirements, clear in structure and delivery, and includes 
reasonable visualizations. 
Written description is similarly clear and in line with length expectations.

*  **Below**: Presentation is well out of line with time requirements, delivered poorly, confusing, or lacking in visualizations. 
Written description is unclear and poorly structured.
*  **Above**: Presentation has exceptional delivery, extremely clear structure, compelling in narrative and 
selection/construction of visualizations throughout. Slides are beautiful in style and design, carefully curated to 
draw attention to key information and complement the verbal delivery.  

