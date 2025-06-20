Configuration in Audioliz
=========================
1. Create a question
--------------------

You can modify/create as many questions as you want in your monitoring sheet. There are three types of questions:

1.1 Question Text
~~~~~~~~~~~~~~~~~

You can choose a question text when the answer is a paragraph. For example: 'Give me the summary of the call' or 'What topics were discussed in the call?'

If you have a yes/no question, it is preferable not to select this type of question.

Let's create a question text:

.. raw:: html

   <div style="text-align: center;">
     <video width="640" height="360" controls>
       <source src="_static\create_question_text.mp4" type="video/mp4">
     </video>
   </div>

1.2 One choice question
~~~~~~~~~~~~~~~~~

A single choice question is used when there is only one possible answer. It's usually used with yes/no questions.

Let's try it:

.. raw:: html

   <div style="text-align: center;">
     <video width="640" height="360" controls>
       <source src="_static\create_question_ONE CHOICE.mp4" type="video/mp4">
     </video>
   </div>

1.3 Multiple choices question
~~~~~~~~~~~~~~~~~

A multiple choice question is used when the answer is not necessarily unique. In this case, you can have multiple answers.

Let's see an example:

.. raw:: html

   <div style="text-align: center;">
     <video width="640" height="360" controls>
       <source src="_static\create_question_MULTIPLE CHOICES.mp4" type="video/mp4">
     </video>
   </div>

To modify a question, it's very simple. Just click on it and change the fields that you want to modify.

2. Change monitoring sheet parameters
-------------------------------------

You can change many parameters in your monitoring grid. Let's see how:

.. raw:: html

   <div style="text-align: center;">
     <video width="640" height="360" controls>
       <source src="_static\action.mp4" type="video/mp4">
     </video>
   </div>
3.Managing Metadata in Audioliz
--------------------------------

3.1 Adding or Modifying Metadata
~~~~~~~~~~~~~~~~~
Metadata refers to additional contextual information attached to a call (such as campaign name, CRM ID, or channel). 
Some metadata is automatically stored in the `crm_metadata` field in the database, but you can also define and manage **custom metadata fields** for specific actions.

To manage metadata for a specific action:

- Go to the **Actions** page
.. raw:: html

   <div style="text-align: center;">
     <img src="_static/choisir_page_action.png" width="550" alt="Dashboard list">
   </div>

- Select the action you want to configure  
.. raw:: html

   <div style="text-align: center;">
     <img src="_static/choisir_action.png" width="550" alt="Dashboard list">
   </div>

- Open the **Metadata** tab
.. raw:: html

   <div style="text-align: center;">
     <img src="_static/choisir_meta.png" width="550" alt="Dashboard list">
   </div>

There, you can:

- ➕ **Add a new metadata** by clicking the plus icon (`+`)  
.. raw:: html

   <div style="text-align: center;">
     <img src="_static/ajouter_meta.png" width="400" alt="Dashboard list">
   </div>

- ✏️ **Edit existing metadata** by clicking directly on the metadata line

For each metadata field, you can define:

.. raw:: html

   <div style="text-align: center;">
     <img src="_static/creation_meta.png" width="550" alt="Dashboard list">
   </div>


- **Name**: The internal name of the metadata, displayed in the **Actions** page.

- **Label**: The display name shown in the **Call Page**.

- **Group**: The section of the **Call Page** where this metadata will appear.

- **Default value**: The fallback value used if the metadata is missing or empty in the call data.  

 💡 **Tip**: If you want the question to be asked — that is, *included in the prompt sent to the AI* — even when the metadata is present but its value is empty (i.e. the field is defined for the call but has no value), then set the **default value to a single space (`` ``)**.

   This ensures that the metadata placeholder will be replaced by an empty string, and the question will not be skipped during analysis.


3.2 Why Metadata Matters in Questions
~~~~~~~~~~~~~~~~~
Some data needed for a question (like a campaign name or product type) varies from one call to another. Instead of creating multiple versions of the same question, you can **insert metadata dynamically** using the `$` symbol in the question text.

Example:
What arguments were given for campaign $CAMPAIGN_NAME?
