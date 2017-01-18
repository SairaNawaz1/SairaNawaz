# Project Design Writeup and Approval Template

Follow this as a guide to completing the project design writeup. The questions for each section are merely there to suggest what the baseline should cover; be sure to use detail as it will make the project much easier to approach as the class moves on.

### Project Problem and Hypothesis
* What's the project about? What problem are you solving?
This project will address what are the major demographic and county-level predictors of suicide attempts in the state of Arizona from 2009-2014 (excluding 2013 because of data issues).

* Where does this seem to reside as a machine learning problem? Are you predicting some continuous number, or predicting a binary value?
This is a predictor of a binary outcome of attempted suicide, ie what is the probability or odds of attempting suicide given a set of demographic and county level variables.  

* What kind of impact do you think it could have?
Recent studies have shown that the rates of self-injury and suicide - especially among youth - are increasing.  So suicide prevention efforts are paramount.  However, there is limited information on how to accurately reflect impact.  This project looks at expanding the definition of impact to include both suicide mortality (which is often easier to come by) and suicide attempts (which is more difficult) 

* What do you think will have the most impact in predicting the value you are interested in solving for?
As mentioned earlier, these data will help determine a better measure for suicide attempts, and then can be used to 1) predict suicide mortality 2) be used as an outcome to see which demographic and county level variables are linked to outcomes
### Datasets
* Description of data set available, at the field level (see table)
The Dataset is the Health Care Utilization Project for the state of Arizona 2009 - 2014.  It includes all hospital discharges and a selection of variables - diagnosis, demographic data, and hospital variables. 
* If from an API, include a sample return (this is usually included in API documentation!) (if doing this in markdown, use the javacription code tag)

### Domain knowledge
* What experience do you already have around this area?
I am a health services research, with training i behavioral health.  Also, I've been working on this project for the past 4 months. 
* Does it relate or help inform the project in any way?
Yes, this project will support some of our later work which will pull from both Emergency Department and Inpatient data.

* What other research efforts exist?
Our Principal Investigator followed a similar methodology using suicide mortality (instead of suicide attempts) to assess the impact of a suicide prevention program in various counties.  However that approach used more national samples of data.  This is the first time we're using a census of all hospital discharges. 

### Project Concerns
* What questions do you have about your project? What are you not sure you quite yet understand? (The more honest you are about this, the easier your instructors can help).
I am still concerned about the extent of predictors I have. Also, the data I have is quite large and I'm not sure where to store it so that I can pull it into the analysis

* What are the assumptions and caveats to the problem?
    * What data do you not have access to but wish you had?
    This represents data in one state over a period of time.  It only includes discharges, which in itself is fairly biased.  We do not know of suicide attempts that did not result in a hospital admission. Furthermore, the predictive model/machine learning will be restricted to a single state
    
    * What is already implied about the observations in your data set? For example, if your primary data set is twitter data, it may not be representative of the whole sample (say, predicting who would win an election)
As mentioned before this data is restricted to individuals who are admitted in the hospital, and excludes those suicide attempts that don't result in hospitalization. Also, hospital data in itself can be biased because some individuals are more likely to visit the hospital compared to others.  Also as this is restricted to one state.

* What are the risks to the project?
    * What's the cost of your model being wrong? (What's the benefit of your model being right?)
    The benefit of a good predictive model is 1) we would be defining the variables for self harm appropriately 2) if a good predictor, we can assess what factors are associated with the outcome
    
    * Is any of the data incorrect? Could it be incorrect?
    We've had discussions with the data providers to ensure the data is accurate.

### Outcomes
* What do you expect the output to look like?
The output would include 1) hospitalizations for suicide attempts 2) hospitalizations for suicide attempts by characteristics 3) rate of hospitalizations by  100,000 4) regression to predict suicide attempts 5) regression of suicide attempts on suidice rates (how well does self harm predict suicide - reliability measure)

* What does your target audience expect the output to look like?
the audience would perhaps like to see the impact of the intervention on the suidice rates.  However measures of the program are needed prior to conducting those analysis .

* What gain do you expect from your most important feature on its own?
As mentioned, understanding how to broaden the measure of suicide to include suicide attempts (as a measure of injury/mental health) is in itself a strong contribution to the field.  Using machine learning to assess the predictors is also an important finding.

* How complicated does your model have to be?
I would like to possibly use different techniques like decision trees to assess this information.

* How successful does your project have to be in order to be considered a "success"?
Applying new techniques - such as decision trees - could be an interesting way to present findings to individuals who typically use other methods (ie logistics and other models) to assess outcomes. 

* What will you do if the project is a bust (this happens! but it shouldn't here)?
I think there's already been much learning in terms of defining ICD-9 codes, learning about new methodologies for validating measures, and using large databases that lend themselves more to learning. 

Saira
