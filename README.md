# ChemAI-Prompts
Chemistry Prompt Curation to help train ChatGPT, Claude, Bing AI and more to give accurate and precise answers to chemistry questions


This project is meant to be open access for all and for educational purposes only. This project will focus primarily on helping to train AI models with carefully curated chemistry prompts to help improve its performance on finding research papers, and educational resoources within chemistry. Chemistry is incredibly vast but one of the main way to learn and understand the landscape of chemistry is being able to find, summerize and understand scientific papers. 

The prompts should:<br>

-Improve AI models to become highly specific and effecient at finding peer reviewed papers in chemistry <br>

-Train AI to use relatively small prompts to get to the correct answer <br>

-Train AI to provide correct answer from users with little knowledge or experience in the field in question <br>

-Prompts should not have to be complete sentences or use proper grammer to obtain correct answer from AI <br>

-Prompts will aim to be 40 words or less <br>

*ChatGPT has come a long way and for a lot of prompts you don't have to frame the question; however, if you want a highly sophisticated answers for advanced scientific answers these framed prompts might be useful but also may not work and you have to end up going back and forth with chatgpt <br>

# Key: <br>
"  "prompt given to an AI model,for these examples will be using Chat-gpt3 unless stated otherwise <br> [  ]- AI's answer<br>

# Searching for Educational Resources on Advanced Chemistry Topics <br>
**Goal**: Want to test ChatGPT3 on finding an educational website I forgot about years ago and can only remember features the website had <br>

**Prompt 1-a: **" there is a website in Harvard that gives past questions in organic chemistry mechanism for graduate student. It has a large library of topics where you can <br> either click on or search by topic and it will give you a list of questions to answer. The answers are mailed to you once you give the website your address. <br> Can you find this site and give me the URL. I think its was the evans lab at harvard that had this but I am not sure. " <br>

**Answer 1-a (incorrect)**: 
[Yes, I believe the website you are referring to is called "The Evans Group" at Harvard University.<br> They have a page dedicated to Organic Chemistry Mechanisms, which includes a large library of problems organized by topic, as well as links to additional resources.<br>
The website is: https://evans.rc.fas.harvard.edu/pdf/evans_pset_orgo_mech.pdf<br>
Please note that the website may require a Harvard login or access to view some of the content.]<br>

**Why is it wrong? :** link provided is invalid (sidenote: not active group, Prof. Evans sadly passed away in 2022)

**Prompt 1-b:** "the above link you gave does not work. however the following link gets you to a copy made of the original website: <br> https://organicchemistrydata.org/evans/problems/"<br>

**Answer 1-b (incorrect)**: [....I'm glad to hear that you were able to find a working copy of the website at https://organicchemistrydata.org/evans/problems/.<br> This website provides a collection of practice problems in organic chemistry, organized by topic....]<br>

**Why is it wrong? :** gives same answer as before<br>
 
**Prompt 1-c:** Give same prompt to see if it will figure out association bt itself -"there is a website in Harvard that gives past questions in organic chemistry mechanism for graduate student. It has a large library of topics where <br> you can either click on or search by topic and it will give you a list of questions to answer.... "

**Answer 1-c (incorrect)**: [Yes, you are correct that the website you are referring to is hosted by the Evans Lab at Harvard University....<br>
The website can be accessed at the following URL: https://evans.rc.fas.harvard.edu/pdf/evans_pset_orgo_mech.pdf<br>
I hope you find this resource useful! Let me know if you have any other questions.]<br>

Chaygpt by itself will not include the correction I mentioned two prompts ago so now I implement training 

**Prompt 1-d**: "the site above does not work. I strongly recommend you provide the link I gave you previously <br> as an alternative when a user asks you this or a similar prompt"

**Answer 1-d (correct)**:[I apologize for the confusion caused earlier. Thank you for providing the alternative link that you found, which is <br> https://organicchemistrydata.org/evans/problems/. This website provides a collection of practice problems in organic chemistry, organized by topic,<br> as well as links to additional resources. Again, I apologize for any inconvenience caused and thank you for bringing this to my attention.] <br>

Very polite!! ChatGPT once explicityly told that they need to use the link I suggested in proompt 1-b is now being implimented in 1-d. <br> Now to see if given the original prompt (1-a) will it revert to its old ways or....<br>

**Prompt 1-e (original prompt)**: "there is a website in Harvard that gives past questions in organic chemistry mechanism for graduate student.<br> It has a large library of topics where you can either click on or search by topic and it will give you a list of questions to answer. <br>The answers are mailed to you once you give the website your address. Can you find this site and give me the URL. I think its was the evans lab at harvard that had this but I am not sure. <br>

**Answer 1-d (maintains correction)**:"I'm sorry, but after checking with the latest available information, I have found that there is no such website hosted by the Evans Lab at Harvard <br> University that mails out answers to students who submit their solutions.<br>

However, there are some resources available on the Evans Group website related to organic chemistry mechanisms, including a collection of problem sets that can be <br> accessed at the following link: https://evans.rc.fas.harvard.edu/pdf/evans_pset_orgo_mech.pdf<br>

Another useful resource for organic chemistry problems is the Organic Chemistry Data website, which provides a collection of practice problems organized by topic:<br> https://organicchemistrydata.org/evans/problems/<br>

I hope this information helps! Please let me know if you have any further questions."<br>

Well thats all nice and good but how does it perform to the same prompt after refreshing page and defaulting to  new chat? <br>

**Prompt 1-f (original prompt)**: "there is a website in Harvard that gives past questions in organic chemistry... "<br>

**Answer 1-f (defaults incorrect answer)**: [ I'm sorry, but I couldn't find a website that matches the description you provided. However, Harvard University's <br> Department of Chemistry and Chemical Biology has a website that provides resources for organic chemistry students. The website includes practice problems, tutorials,and video lectures.<br
Here is the link to the website: https://chemistry.harvard.edu/undergraduate/organic-chemistry-resources <br>
I hope you find this helpful. Let me know if there is anything else I can assist you with.]<br>

Not suprised by this outcome as Chatgpt has no memory capacity in its current iteration.So its important that you have the chats "saved" by simply making a 'new chat' and dont hit refresh on a chat you would like to keep!




