## Speaker Notes

### Introduction
**Introduce Myself**

Today I would like to discuss how AI can be used by faculty to improve our teaching.

I am going to start with telling you about how I am using it in my courses, and then I will show you how to create a simple interactive tool using AI.

Hopefully, at the end there will be time for questions and discussion. However, feel free to ask questions at any time.

### Some Use Cases
Like many of you, I have been using AI to help me become a better instructor.

I have been using the tools as a helpful assistant, never as the primary source of content.

I am only good at a few things (writing programs and teaching others to write programs) and I believe that a generic AI model is not better at those things than I am. However, there are some things that an AI assistant can help me do better.

I do things like:
- Have an AI model look at my lecture notes to clear up any confusing language, make them more concise, and look for important elements that are missing.
- Ask for ideas about in class activities and assignments.
- Generate questions for written exams and quizzes. Sometimes this is coming up with distractors for multiple choice questions, and sometimes it is generating open ended questions.
- Ask the AI models for advice and general help with teaching. It often will give me an unbiased and helpful perspective on how to approach a problem.

I do not do things like:
- Ask an AI model to write my lecture notes for me.
- Ask an AI model to write code that I will present in class.
- Ask an AI model to grade anything for me.

In other words, I use AI in areas where I don't feel very confident. I don't use it in areas where I do feel confident.

### Setting Expectations
Since last semester I have been very clear with my students about how they can use AI with their work. I post this information on each assignment's description on the LMS. I also talk about it in class and have a discussion about it.

I created a tool to help me generate the language for these policies. 

[Show AI Policy Generator](https://markm208.github.io/aiPolicyGenerator/ai-policy-generator.html)

You'll see in a moment that I created this tool using the same 'hands-off' process that I am going to show you how to do today. 

[Show Assignment Description 1](https://lms.carthage.edu/assignment/8181773963/info)
[Show Assignment Description 2](https://lms.carthage.edu/assignment/8194520110/info)
[Show Assignment Description 3](https://lms.carthage.edu/assignment/8207255570/info)

I have found that students feel relieved to have clear guidelines about how they can use AI. 

It also helps them understand that I am not trying to catch them doing something wrong, but rather I am trying to help them use the tools in a way that is ethical and beneficial for their learning.

### Building an Interactive Tool
The main focus of this session is to show you how I use AI coding assistants to build interactive tools for my courses.

It turns out that you don't need to know how to code to do this. You just need to be able to have a conversation with an AI model and be able to copy and paste some code into a file.

I have been using this process to create simulations, visualizations, and step-by-step demonstrations for my courses. 

These are things that I can explain in a more traditional lecture format (and have done many times in the past), using a whiteboard or slides (or with just a lot of hand-waving). These are low stakes demonstrations that help students visualize something that is traditionally hard to see about software development. 

These are not the most critical learning experiences that I teach in my courses, for those things I rely on my own expertise and experience. However, these tools are a nice *supplement* to my lectures and help students understand the material better.

As I mentioned earlier, I use an AI coding assistant to help me build these tools. 

I could have written the code for these myself, but it would take me a lot longer to do it. 

These are not important enough learning experiences for me to do it by hand. The great thing about these coding assistants is that they can create visually appealing and interactive tools with very little to no 'hard' coding on my part.

These tools do not have a lot of complex logic, they are just a clean way of showing some steps (UI is not my strong suit and this is not where my confidence lies).

For the really important concepts I have other materials that I have created for more than two decades. I don't rely on AI to build those materials for me.

### Example Tools
Let me start by showing you an example of a tool that I created for my courses. This is a tool that helps students understand how to use the 'git' version control system.

[Show Git Tool](https://markm208.github.io/vibeCodingInClassTools/git-workflow-simulator.html)

The important thing that I am trying to show in this example is the flow of work on a team of software developers. 

If you are teaching accounting or costume design you will definitely have a different concept that you want to demonstrate, but the process of building the tool will be the same.

#### Demo 1
- click through all of the buttons to visualize the workflow
- on the left is a preview of what they should expect
- on the right is a log of what happened with explanations
- I discussed all of these steps in a lecture, then before we practiced with the actual tools I had them use this tool with a partner to get them used to these complicated workflows

#### Demo 2
In this next example, I am showing the students how to work from the terminal. I start with a lecture about how using the terminal is like a hiker climbing a mountain. When I was working with the AI coding assistant I gave it my lecture notes and described the analogy and the technical concepts that I wanted to demonstrate.

[Show Terminal Tool](https://markm208.github.io/vibeCodingInClassTools/cli-hiker.html)

I used to present something like this:

https://docs.google.com/document/d/1Q7dFUhyGjCCgxVFhZi2wo5WByMzKyGy2scUkBhFEyAk/edit?tab=t.0

and then walk through it using my computer and a projector. Then, I'd have the students work on a 'lab' problem on their own computers. 

Now, I have them use this tool to get used to the concepts and the workflow before they start working on the lab problem.

### Building a Tool from Scratch
The way that I use the AI coding assistants is to start with a request for a single page web app that uses html, css, and javascript. I ask it to have a particular look and feel and then I ask it to satisfy some particular requirements that I have for the tool.

I then have a conversation with the model about how to improve the tool and add features to it. So far, it has never been able to get everything right on the first try. I often have to ask it revise its work 20-40 times before I am happy with the result.

Here is the log of my conversation with the model as I was building the terminal tool:

1. I am working on a command line tutorial for my operating systems course. The file 03_CLITutorial.md has the basics. I was hoping you could write a single page web app using html, css, and javascript that builds on the mountain hiker analogy that I mention in the tutorial. Feel free to build pngs or svgs to help visualize the concepts.
 
I have another program that I really like that I'd like you to look at and make it feel similar. That program can be found here: '/Users/mmahoney/Dropbox/vibeCodingInClassTools/git-workflow-simulator.html'.
 
Can you come up with a few ideas about what you are capable of building? 

---

2. Combine the best elements from the proposed ideas and show me what you come up with. You can create a new directory in code-examples called 'hikingCLI' and put all of your work in there. 

---

3. Great! When a user creates a new directory I noticed that a new node doesn't show up on the mountain (but it is in the file system view).

Also, the whole mountain pic feels a little cramped, can you make it a bit wider or bigger? 

---

4. There seems to be a hover effect when I cd that covers up the name of the directory. Can you get rid of that? 

---

5. Sorry, I think I misspoke. It is the feature that lists the location that moves with the picture of the hiker.

---

6. It is the location-label that I am talking about. I don't think that it helps.

---

7. The 'peak' directory is a little hard to see along with the root. Can you get rid of the peak and adjust everything else that is dependent on it being there? 

---

8. In the file tree, when I hover over a file can you bring up a dynamic view of the text or contents of the file? 

---

9. In the trail guide, if the operation has not been completed when a user clicks on an element can you issue the command in the terminal for them?

---

10. What is secet about the cave?

---

11. Can you make the scroll a hidden file and give the user a hint about how to read it? 

---

12. Can you change it to 'discover the secret in the cave' and once the user moves there give a message about the contents of hint.txt being something they should read via cat? 

---

13. What would normally be the path for most of these commands? Can you add them to that directory and add an echo $PATH option so the user can see where the commands are? 

---

14. Can you add an item to the trail to ask the user to display the $PATH? 

---

15. Sorry, I still want them to echo the path first and then print out which ls is being used. 

---

16. Can you make the file tree collapsable when you click a directory name? Also, only have the hiker directory open by default 

---

17. In the 'Your Backpack (PATH)' when you hover over the names of the commands can you display the location of the commands and a brief description of what they do? Also, get rid of the 'Quick Reference' since this new feature will act as it. 

---
18. Can you put the current-location element right about the text 'Map (File Tree)' and label it 'Current Working Directory' 

---

19. Right now it looks like the hiker directory is the home dir, is that correct? Are all user's homes inside home?

---

20. In a few places you used markdown syntax in the display of commands. For example, you display "Type pwd to see your current location." I want to make sure that the students know that you don't type the back ticks. Instead of surrounding the commands with back ticks can you apply a style to those elements so that they look like code being typed in the terminal? 

---

21. Can you improve the image of the hiker to make it a bit more sophisticated? It looks almost childlike now.

---

22. In the file tree it looks like there should be a directory called 'bin' inside /usr/local but when navigating it doesn't look like it is there. Can you check that and all of the other locations in this simulation to make sure they are accurate?

---

23. When displaying the home directory in "Current Working Directory" you are currently using the tilde (~). I wonder if you could use the full path like you do for the other directories and then put a parenthetical tilde next to it?

---

24. In the current working directory display I only wanted the parenthetical output in the home directoy. In all of the other ones, I don't need to refer to the path from the home directory.

---

25. In the display for "Your Backpack (PATH)" can you change this to "Tools In Your Backpack (Available Commands)"

---

26. Can you remove the "(Available Commands)" and make it say that when one hovers over the element. 

---

27. When I hover over the cd command in the "Tools in your backpack" it says "shell builtin" instead of listing the location of the command. Is there a reason why you did this?

---

28. Can you remove cd from the /bin directory then?

--- 

### Live step
29. Add an icon (a gear or something) that when clicked a modal dialog appears with a set of instructions about how to use this tool. Make sure a newcomer will know all of the things that they can do with the tool.


The conversation went back and forth. I can characterize the communication as:
- I started by asking for some ideas without really knowing exactly what I wanted. It built something that was interesting but not what I wanted.
- There was something that was hard to see and I asked it to clean it up. It didn't understand what I was looking for at first.
- I thought of features once I was using the app for the first time and I asked it to add those features. 
- I asked for improvements in the flow of the app and the user experience.

I did not look at the code once (I have still not looked at it). The AI assistant wrote it all to a single html file that I opened with my browser and then I had my conversation about it.

You can do the same thing. You can start with a simple request for a single page web app that demonstrates a concept that you want to teach. Then you can have a conversation with the model about how to improve it and add features to it.

### Conclusion
I hope that this has given you some ideas about how you can use AI to build interactive tools for your courses. You don't need to know how to code to do this. You just need to be able to have a conversation with an AI model and be able to copy and paste some code into a file.

### Questions and Discussion
I would love to hear your thoughts and questions about this process. 

Would anyone like to work with me on building a tool for one of your courses with the time that we have left?