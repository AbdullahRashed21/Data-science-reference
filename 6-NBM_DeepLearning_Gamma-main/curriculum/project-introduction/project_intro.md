# Deep Learning Project Introduction

## Summary:

Using **primarily non-tabular data** (images, text, time series, audio, etc.), build a **neural network model** that addresses a useful prediction and/or recommendation problem in any domain of interest. Communicate your process and findings in a 5 minute presentation (to the entire class at the end of week 2) and a short written description. 

Metis projects are broken down into 5 component parts -- **design**, **data**, **algorithms**, **tools**, and **communication** -- that correspond to the grading rubric and [project success guide](./project_success_guide.md). Below is a description of each component as it relates to this project. For more detail on how these components are graded and how extra points are rewarded, refer to the success guide.  

### Design:

*  The project should be centered around a **well-posed deep learning problem** in a domain of interest that can be reasonably addressed by available non-tabular data
*  All **deliverable deadlines should be met**, reflecting **professionalism** and **effective scoping and workflow**

### Data:

*  The **data must be primarily non-tabular**, from any data source of interest. Acceptable data formats include images, text documents, audio, time series, and videos (consult with an instructor if in doubt). Acquisition options include straightforward downloads, web scraping, use of APIs, [BigQuery public data](https://cloud.google.com/bigquery/public-data) etc.
*  Supplemental data (e.g. supporting tabular information incorporated with an additional network input branch) is always welcome, but not required
*   If able to **leverage transfer learning** (usually applicable for images, including audio spectrograms, or text), aim to have at least **1000 data points for regression** or **several hundred data points per class for classification**. If unable to leverage transfer learning, it is safer to aim for 1000s if not 100,000s of datapoints because neural networks are typically very data hungry. Exceptions to this guideline may be appropriate depending on the domain, but an instructor should be consulted.   
 
### Algorithms

*  Building a **neural network model** in python is required, including the appropriate use of specialized architecture components such as convolutions or recurrent layers to handle the data format 
*  **Rigorous model selection and evaluation** (i.e. proper validation and testing) is required
*  Neural network methods beyond those covered in the course or other additional modeling methods are optional

### Tools

* **Python neural network libraries/tools** are required (primarily keras) 
- Other tools not covered in the course are optional but welcome
  - *Acquisition* tools could include web scraping libraries or use of APIs
  - *Storage* tools could include SQL or noSQL (e.g. MongoDB) databases
  - *Processing* tools could include Google Cloud or Amazon Web Services for cloud computing resources, or format-specialized tools such as librosa (audio) or OpenCV (images)
  - *Visualization* tools could include python libraries such as Bokeh and Plotly or resources outside of python such as Tableau
  - *Production* tools could include Flask or other web app libraries/technologies

### Communication:
 
* Students will deliver a **5 minute slide presentation** at the end of the course. These should be given in a compelling, clear manner and include effective visuals for communicating your objectives and findings
* You will also submit a **~1 page written description** summarizing your work: it should begin with a **~100 word abstract** to be followed by a breakdown of your project along the 5 major components


## Deliverables:

**Please submit all project deliverables through the [Student Submissions Form](https://docs.google.com/forms/d/e/1FAIpQLSeM7MPx5r_FaX6ordJGkG1ObLh94GEE8qzlvEFxfvmWsKmXNA/viewform)**. All project deliverables and code should be uploaded to a personal, project-specific GitHub repository. Click [here](https://github.com/thisismetis/Metis_Fundamentals/tree/main/git_and_github) for instructions on how to set up a personal repo. 

**For exact deliverable dates, refer to the main schedule [here](/README.md).**
  
**For exact deliverable details, refer to the (linked) Metis Fundamentals project deliverable templates**.

 * [Project proposal](https://github.com/thisismetis/NBM_Metis_Fundamentals/tree/master/project_deliverable_templates/project_proposal.md): short description shared with instructors
    - Additionally, students may meet with an instructor for a scope meeting
 * [Minimum Viable Product (MVP)](https://github.com/thisismetis/NBM_Metis_Fundamentals/tree/master/project_deliverable_templates/mvp.md) submission  
 * [Written description, presentation slides PDF, and project code](https://github.com/thisismetis/NBM_Metis_Fundamentals/tree/master/project_deliverable_templates/final_deliverable.md) 
 * Project presentation


## Example Project Ideas
- Image Classification: brand logo detection in social media posts
- Image Classification/Recommendation: clothing image-based recommendation  
- Text Classification: detect abusive social media comments 
- Audio Classification: detect heartbeat arrhythmia    
- Time Series Forecasting: multi-station transit data, bikeshare usage patterns 
- Time Series Forecasting: demand forecasting for large number of products
- Image Captioning (Challenging): map input image to text description
