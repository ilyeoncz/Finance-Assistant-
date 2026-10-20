Developers Diary
20/10 4:39pm - I wrote my developers diary on Word, and after double checking the project specifications I've realised that it is meant to be as part of my repository.

10:06 am 4/09/26

<img width="940" height="300" alt="image" src="https://github.com/user-attachments/assets/9c56e3ee-120a-44ec-bc46-ef53ac9e4cf0" /> 

I am working on beginning my tracker based off code we studied in Module 2. This is just so that I have something to go off. I am likely to get rid of this or change it in future. 

10/09/26

12:19pm

<img width="940" height="293" alt="image" src="https://github.com/user-attachments/assets/12c4b11d-bfee-4ee4-8b5c-96a9110802ce" />

I decided to restart and rather than doing an interface, I start with an introduction to set out the guidelines for the financial assistance.

12:32pm 

<img width="940" height="221" alt="image" src="https://github.com/user-attachments/assets/fd6bacaa-6fca-41e3-9be5-f47d69785a5f" />

I tried to copy my code from module 1 except I found that it wasn’t super clear whether it wanted expense names or expense amounts, I am going to try and clear this now 

12:37pm

<img width="659" height="128" alt="image" src="https://github.com/user-attachments/assets/0657c200-5e4b-47d4-9628-d0ad8cd03081" />

I’m trying to think of how to prompt and organise categorising on monthly expenses before organising the costs 

15/10/26

11:50am 

<img width="940" height="278" alt="image" src="https://github.com/user-attachments/assets/38a8fb74-c9fd-4a93-b063-fd78241b0395" />

I forgot to save my project and now I am restarting 
 
20/10/26

12:40pm

<img width="940" height="413" alt="image" src="https://github.com/user-attachments/assets/2742027f-dab1-4a42-b183-c90a3a7e0723" />

I have just imported datetime so that my session displays the time it was started and I am now getting assistance from AI so that I can categorise the expenses as low, moderate and high. This will be used to give users of the financial assistance an idea of how each of there expenses sit in the budget. I am taking this as inspiration from module 5.

1:01pm 

I read the project specifications properly now and realised I forgot to import all of my key functions before starting the code
Now that I have imported pandas, a Gemini API key and Gradio it will be easier to organise and write my code. 

<img width="940" height="386" alt="image" src="https://github.com/user-attachments/assets/26b0eaf4-e960-4b36-be71-78e65ff63456" />
Yay

1:39pm

<img width="940" height="438" alt="image" src="https://github.com/user-attachments/assets/f13d82c0-36d1-4dc2-a1e5-63d9e56464f7" />

I asked Gemini to help me allow the user to choose their own colour for the interface 

2:26pm

I pasted all of my code over the semester into gemini and asked it to unify it all into one tracker. 
I had to refine it with multiple prompts, but after 5 attempts. This is what I have right now. 
I am going to go through now line by line and edit and refine the code.

<img width="940" height="628" alt="image" src="https://github.com/user-attachments/assets/07658597-ec21-4f78-8460-7e90d264ad03" />
<img width="993" height="616" alt="image" src="https://github.com/user-attachments/assets/e971007c-6981-4515-a50f-44639cada3bb" />

I still wanted to keep the colour personalisation function in my code, which Gemini didn't have. I asked how to integrate it into this code so that there was still an option of personalisation for the users!


<img width="946" height="641" alt="image" src="https://github.com/user-attachments/assets/ddb0b292-2ea6-4593-b0be-2535b5d23e87" />

I ended up ignoring this and copying what I did in module 8 

<img width="1002" height="291" alt="image" src="https://github.com/user-attachments/assets/649f2157-52f2-4fed-8c04-75e423c886b4" />
<img width="940" height="842" alt="image" src="https://github.com/user-attachments/assets/2f95ae7d-0a6e-4121-bf0b-b7d664321e63" />
<img width="940" height="378" alt="image" src="https://github.com/user-attachments/assets/336abe1c-1a2d-4acb-acae-f6bff7c287eb" />  
<img width="446" height="291" alt="image" src="https://github.com/user-attachments/assets/6d5f81a3-c42f-4c5a-8bf4-e4015d6eca73" />

When I copied module 8, I did have to update the API to gemini-3.8-flash
Eventually I managed ask multiple prompts to refine the code to make sure that it only included information I had learnt over the semester, whilst also adding my own touches from what stood out to me after everything I was taught. 


4:01pm

<img width="940" height="374" alt="image" src="https://github.com/user-attachments/assets/7d53a163-9e71-4eef-bb84-80a776435941" />

Originally the user_transactions = [] was underneath global user_transactions at the top of the test run 
This was showing up in my Gradio website before as an included expense when I was testing the new code, so I needed to make sure it wasn’t being included as an additional expense anymore.

4:47pm

<img width="1900" height="1052" alt="image" src="https://github.com/user-attachments/assets/23e89cdb-51dc-4089-8f78-ec67e1a948b0" />

I finished pasting my developers diary into my GitHub repository... Making sure to save everything this time.

5:07pm

<img width="1002" height="491" alt="image" src="https://github.com/user-attachments/assets/5ea9c59d-9a11-46bc-bb07-6748769929ed" />
<img width="955" height="801" alt="image" src="https://github.com/user-attachments/assets/f7d00299-a298-49df-9c14-9c7c68999b9b" />

I didn't really understand how the API key worked or prompting the AI so I asked Gemini to explain each line for me so that I knew what each line meant in case I wanted to change anything.
I discovered that this code converts the pandas table, the monthly budget and the expenses into data for the AI agent to analyse. The code then prompts the AI so that it only responds as if it is a "helpful, realistic personal financial coach," ensuring that gives an appropriate AI analysis. 
The last line of this code also ensures that if there are any errors with the AI, it will print an error message, rather than crashing the whole code.

21/10/25
12:56am

<img width="1738" height="708" alt="image" src="https://github.com/user-attachments/assets/05b26b15-6b81-4e20-b9d7-eaa46199be03" />

I am trying to make it so my API key can respond to questions rather than just answering the predetermined prompt, but I keep getting and error so I am going to try to fix that now.

1:01am

<img width="1121" height="517" alt="image" src="https://github.com/user-attachments/assets/c7598df8-fee9-4097-94bc-095948429578" />

I tried to add the AI code in this section, which I have deleted and I asked Gemini why that wasn't working and it recommended for me to copy what I have done here except instead of "generate_ai_feedback" I could use "ask_custom_ai_advice" so that there is two sections that dont interfere with one another and fulfil their individual task.

1:16am

<img width="738" height="297" alt="image" src="https://github.com/user-attachments/assets/9c4cf399-a6cc-49c0-9335-0d14163f01ce" />

I got an error code :(

1:17am

<img width="1531" height="583" alt="image" src="https://github.com/user-attachments/assets/ce698e8d-58e3-4686-8b4d-7aaa0e97de4d" />

I tried asking AI a question not related to the task and it still responded appropriately meaning that it is now functioning correctly!

Because we had to add two unique aspects to this financial assistant, one of mine was to make the theme personalised, and another was to give AI feedback based off the prompt I created.

I am really happy with this finance tracker now and will spend tomorrow night fixing anything!
