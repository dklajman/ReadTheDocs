Comments and Feedback
=====================

1.How to add a comment to an analyzed record ?
---------------------------------------------------

You can add a comment either at the level of the responses to each question or in the comment field located right after the transcript.and you need to follow the following steps: 

- Choose a status for the comment in the DEBUG-STATUS field, the status must be :
       |$|OPEN|$| when you ask a question or leave a comment
       |$|REPLIED|$| when someone responds to your comment
       |$|CLOSED|$| when you have the correct answer to your comment
- choose the Importance level of your comment: 
       Normal
       Medium 
       High

(vidéo)

2. How to find and respond to comments left on an analyzed call ?
---------------------------------------------------------------------

You need to click on the "comment" field, a tab will open where you can filter by call date, agent, CRM ID. 
To find the comments left, click on the "DEBUG STATUS" field and select the "OPEN" option to display all the analyzed calls where a comment has been left. At this point, you have the option to quickly view all comments left on calls by clicking on the two arrows next to "👁️‍🗨️". Or reply to the comments by clicking on "👁️‍🗨️", opening the call analysis grid, and following these steps:

- Change the "DEBUG STATUS" field to "Replied" 
- Select the person responsible for the response in the "IN CHARGE" field.
- Reply to the comments and questions in the "ANSWER" field.

(vidéo)









3. Supervision and Question Adjustment Process
---------------------------------------------------------

3.1. Continuous Improvement of Question Formulation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As part of our continuous improvement process, we aim to refine the way questions are written. This effort involves both our internal team and the client, as misunderstandings about the client's actual needs can also lead to discrepancies.

To address this, we have implemented a parallel procedure on the client’s side:

- A supervisor reviews and corrects incorrect answers manually for specific questions.

- The supervisor must fill in the **Counter evaluation by** field with their name.

- They are also encouraged to add comments explaining the corrections made.

On our side, we are committed to adjusting the relevant questions based on the supervisors’ feedback, with the goal of minimizing the gap between the AI’s analysis and the human evaluation — a goal that we actively monitor through the AI / HUMAN page on our BI dashboard.

.. image:: /_static/ecart_ia_hum.png
  :width: 600
  :alt: Dashboard list


3.2 Evaluation and Supervision Process
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
To ensure the quality and accuracy of AI-based analyses, supervisors on the client side are expected to review and validate the AI's responses for specific calls. The following steps outline the recommended evaluation procedure:

- Access the call page that needs to be reviewed.

- Fill in the **Counter evaluation by** field with the supervisor’s name.

.. image:: /_static/champs_a_remplir.png
  :width: 600
  :alt: Dashboard list



To help our team better understand the corrections, it is strongly encouraged to add a comment in the following format:

- question_name: incorrect AI answer → correct answer | reason for the change

.. image:: /_static/image_2025-06-18_141937013.png
  :width: 600
  :alt: Dashboard list

In addition, the supervisor should review the AI-generated responses, click on any incorrect answers, and manually correct them. They can also leave a more detailed comment on each question if needed.

.. image:: /_static/changer_question.png
  :width: 600
  :alt: Dashboard list


4. Understanding the IA vs Human comparison dashboard
---------------------------------------------------------

This page allows you to explore the differences between evaluations made by the AI and those made by human reviewers.

1. Score Table
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


This table displays, for each counter-evaluator and each call, the human score, the AI score, and the difference between the two.
If a counter-evaluator (e.g. Hayat) does not appear, it means no human score has been recorded for the selected period or filters.


.. image:: /_static/Score_Table.png
  :width: 800
  :alt: Score table by counter-evaluator

2. Evolution of the average gap between IA and human scores
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This graph shows the trend of the average difference between the human and AI scores over time (day, week, or month depending on filters).

.. image:: /_static/Evolution_of_the_average_gap_between_IA_and_human_scores.png
  :width: 800
  :alt: Line chart showing average gap over time

3. Question-wise Accuracy Table
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This visual presents, for each question, the percentage of correct and incorrect responses by the AI (based on human validation) per counter-evaluator.

.. image:: /_static/Question-wise_Accuracy_Table.png
  :width: 800
  :alt: Accuracy per question and reviewer

4. Call-by-Call Details
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This detailed table shows the call ID, agent name, counter-evaluator, the evaluated question, the human answer, the AI answer, and whether the AI's response was correct or not.

.. image:: /_static/Call-by-Call_Details.png
  :width: 800
  :alt: Accuracy per question and reviewer




