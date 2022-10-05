# Deep Learning Course Project Success Guide

Metis projects are grade by point assignments for five component parts, each on a scale of 1 to 5.
A score of 3 on a component indicates that the project requirements for that component have been well met,
while scores below and above 3 respectively indicate that requirements are not met or are significantly exceeded. 
The components are: **design**, **data**, **algorithms**, **tools**, and **communication**. A total score of 15 (average of 3 per component) is required to successfully pass the course.

For specific instructions on this project's requirements, refer to the [project introduction](./project_intro.md). 
Below are guidelines mapping out the typical project factors in each component that lead to a score of 3, as well as those that help contribute to being below or above a 3. 
**Note that these factors are guidelines and are not prescriptive**; instructors will ultimately grade based on their careful judgement in conjunction with these guidelines, 
so it is not a good idea to try to "game" these guidelines. 

If in doubt about expectations or a score received, you may always consult the instructional team.

**Important note on deliverable deadlines**: Refer to the [daily schedule](../../README.md) for all project deliverables and their deadlines, both intermediate (project proposal, MVP) and final (slides, writeup and code). If you submit your final deliverable later than 11 am ET on presentation day, you will receive a 1 point penalty under the Design category. If you don't submit by 3 pm ET on that day, **we will not be able to grade your project and you will not pass the course**. Any exceptional circumstances should be discussed with your instructors and program manager as soon as possible. You should also meet the intermediate deliverable deadlines  -- your ability to keep to deadlines and display professionalism in your project work will be scored under the design category.

### Design:

*  **Satisfactory**: Includes a properly framed, useful problem addressable with primarily non-tabular data that is appropriately handled with deep learning techniques. All deliverable deadlines are met.  

*  **Below**: Project choice is not appropriate for deep learning methods, non-tabular data is not adequately incorporated, deliverable deadlines are not met.
*  **Above**: Demonstrates exceptional creativity and proficiency in leveraging deep learning techniques to address a complex, useful question involving non-tabular data. 

### Data:

*  **Satisfactory**: Primary data is non-tabular and of adequate size for the deep learning problem being addressed (typically smaller if transfer learning is applicable).

*  **Below**: Primary data is tabular. Data set is small or overly simple. 
*  **Above**: Data is large in scale (e.g. 10,000+ large files such as images).
Data has significant formatting/handling complexities
such as requiring significant, format-specialized processing or extensive preprocessing overall. 
Multiple datasets (potentially including supplementary tabular data or multi-format network inputs) are leveraged via merging disparate sources.  
 
### Algorithms

Note that students **are not graded based on evaluation metric scores**: we are looking for soundness in approach and rigor in exploring the problem you've chosen as thoroughly as possible. Deep learning problems will vary widely in the predictive challenge they pose, and the "success" of a model is contextualized by this level of challenge, not by absolute metric numbers or results. 

*  **Satisfactory**: A deep learning model is successfully built and tuned using a rigorous selection/evaluation framework (i.e. with proper validation and testing and a reasonable choice of metric). Specialized architecture components such as convolutions or recurrent layers are applied as appropriate to handle the data format and model results are interpreted correctly and applied in a useful manner. 

*  **Below**: No deep learning model is built, or the model built is deficient in approach -- e.g., the model is poorly tuned or an inappropriate fit for the problem being addressed.      
*  **Above**: A carefully curated deep learning model is built: rigorous preprocessing and network architecture engineering are performed, with the model's end application always clearly in mind. Meticulous attention is paid to model selection methodology, to the point of considering model scalability. Specialized network components including those beyond the scope of the course are incorporated, their use understood and well-justified by the student.  

### Tools

*  **Satisfactory**: Python deep learning libraries are adequately used to construct a neural network that handles the non-tabular data.

*  **Below**: Python deep learning libraries are not used, or are used in a trivial manner to process supplemental instead of primary data.
*  **Above**: Advanced techniques within Keras or other python deep learning libraries (e.g. PyTorch) are used to implement specialized techniques/architectures and/or to handle significant preprocessing challenges. Advanced tools not covered in the course are used as a significant component of the project.

- Major examples of applicable tools not covered in the course:
  - *Acquisition* tools could include web scraping libraries or use of APIs
  - *Storage* tools could include SQL or noSQL (e.g. MongoDB) databases
  - *Processing* tools could include Google Cloud or Amazon Web Services for cloud computing resources, or format-specialized tools such as librosa (audio) or OpenCV (images)
  - *Visualization* tools could include python libraries such as Bokeh and Plotly or resources outside of python such as Tableau
  - *Production* tools could include Flask or other web app libraries/technologies

### Communication:
 
*  **Satisfactory**: Presentation is in line with time requirements, clear in structure and delivery, and includes reasonable visualizations. 
Written description is similarly clear and in line with length expectations.

*  **Below**: Presentation is well out of line with time requirements, delivered poorly, confusing, or lacking in visualizations. 
Written description is unclear and poorly structured.
*  **Above**: Presentation has exceptional delivery, extremely clear structure, compelling in narrative and selection/construction of visualizations throughout. Slides are beautiful in style and design, carefully curated to draw attention to key information and complement the verbal delivery.  

