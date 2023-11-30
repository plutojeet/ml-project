# botV1

### Brief description of project structure 

1. data folder contains the data set <br>
data/nlu.yml -> dataset<br>
data/rules.yml and data/stories.yml -> rules defined for output of model
2. result folder contains testing results
3. bot.py is the frontend of the project built in streamlit
4. config.yml contains the defination of the machine learning pipeline
5. domain.yml -> configuration file that outlines the AI assistant's capabilities, defining its language understanding, actions, and responses.


# to run 
- Python v3.8
- pip install -r requirements.txt
- In one terminal -> rasa run actions
- in another terminal -> rasa shell

# Intents

- greet
- goodbye
- Auxiliary_exam_process
- General_info
- General_info_Auxiliary
- ask_exam_evaluation_process
- ask_fee_details
- ask_fee_refund
- ask_subject_limitation
- confirm_self_study_conditions
- deny
- entered_grade
- entered_subject
- explain_grade_improvement_process
- inquire_about_grade_upgradation_eligibility
- inquire_about_medal_scholarship_upgradation_criteria
- subject_re_enrollment_auxiliary_yes
- subject_re_enrollment_summer_no

# Entities

- upgradation_mode ( auxilary/summer/backlog)
- grade:
  - roles:
    - current_grade
    - upgraded_grade(Not used anywhere right now)
- subject (subject code )
- study_mode (self / regular)
- marks (not used anywhere right now)
- purpose (registration / tenure_of_summer_term / time_table)
- month
- fee type
