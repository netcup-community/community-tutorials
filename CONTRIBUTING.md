## netcup Community Tutorial Guidelines

# General Criteria 
- Please limit yourself to one tutorial per pull request.
   - It is permitted and encouraged to include both a German and English version of the tutorial in one pull request, however for different tutorials, use separate pull requests.
- Tutorials should be delivered ideally both in English and German, while English is the default language.
   - In the rare circumstance, that you are unable to provide a German translation, we may be able to translate the tutorial internally.
   - To maintain high quality we preserve the right to edit files for better understanding without changing the meaning of your tutorial.
- Name the product you're using.
   - Whether it is Webhosting or a vServer you are using in your tutorial, please make sure to name it. (e.g.: Webhosting 4000)
- Make sure your tutorials work on new servers.
   - If someone has just ordered a new server, they should not have to install or configure anything first, unless it is explained in your tutorial. In that case, make sure there is already a tutorial that explains it and link to it at the beginning of your tutorial.
- Write in a structured, easy to follow manner.
   - Since your content will be read by users with a wide range of experience, make sure beginners can still follow.
   - If you use acronyms, write them out the first time you use them.
   - If you use a word that not everyone is likely to understand, explain it. Or use another word or phrase that is easier to understand.
   - Don't skip steps. Some might seem obvious or self-explanatory to you, but aren't to others.
   - Don't overdo insider jokes. (Looking over to you, dear "Duck-Community". :wink:)
- Be the original.
   - We will not accept tutorials that can be found anywhere else on the web, especially if not in context with netcup.
   - Make sure your tutorial is new to the collection. In case it's not, have a look if it would be a valid expansion of an existing tutorial. In case you found one, don't hesitate to reach out to us.
- Be up to date.
   - If you have already forked the community-tutorials repository, please make sure to fetch the upstream on a regular basis.
- Let us and the community work their magic.
   - After you create a pull request, don't keep editing your tutorial unless we specifically ask you to do so. Otherwise, the review process will take longer than necessary. If you forgot something, either we or the community will notice it and ask you to add the missing information. 
- Submit one tutorial at a time. 
   - To keep our review structured and efficient, you should only submit tutorials that contain one instruction at a time. Don't squeeze several tutorials into one file. You can always submit several separate tutorials.

# How To
1) Fork the project
2) Add your tutorial folder: `mkdir -p community-tutorials/this-is-a-tutorial`  
3) Add the templates: `cat TEMPLATE.md > community-tutorials/this-is-a-tutorial/01-en.md` 
4) Write the content (using the [template](https://github.com/netcup-community/community-tutorials/blob/main/TEMPLATE.md)) 
5) Create a pull request and include the following in your request:

I have read and understood the Contributor's Certificate of Origin at the end of the [template](https://github.com/netcup-community/community-tutorials/blob/main/TEMPLATE.md) and I hereby certify that I meet the contribution criteria described in it. 

Make sure that you have your email address visible on your Github account. If your tutorial is accepted, you will receive an email from our netcup Community Team asking for your netcup Customer-ID, so the reward can be processed.

# Structure
All of your tutorials should have the same basic structure:

- Title
- Introduction
- Steps
- Conclusion
## Title
The title should be a summary that gives users an immediate idea of what the tutorial is about. e.g. Installing <software> on <Operating System>

 ## Introduction
The first few sentences are here for you to explain what your tutorial is about. Make sure to be on point with what users will end up with when they finished your tutorial. Also: let them know if there are special requirements! Link other tutorials that your tutorial builds on, and add recommendations for what users should know.

## Steps
Now we're right in the heart of the tutorial where users will follow every single one of your (foot)steps.
The amount of steps will vary depending on how long or complicated your tutorial is.

Remember: none of the users walked that road before, so make sure to really explain your steps well.
Each of them should build on the previous one. It is important not to skip any steps, no matter how obvious or self-explanatory they may seem! (If you're not sure what we mean here, you might want to watch this fun video: https://www.youtube.com/watch?v=cDA3_5982h8&t=4s)

## Conclusion
Once all steps are completed you might want to add a short conclusion.
You can either summarize what has been done or give the user an overview of what to do next.

# Code Example
You can create code examples in nearly every programming language. Just state the language after the first three backticks in your Markdown file.

``` js
var x, y, z;
x = 5;    
y = 6;   
z = x + y;  // Comment
document.getElementById("tutorial").innerHTML = "The value of z is " + z + ".";
```

# Template
For all of this we provided a template for you. See https://github.com/netcup-community/community-tutorials/blob/main/TEMPLATE.md

It includes:

- a basic layout for your tutorial,
- some examples of formatting,
- tips and tricks for setting everything up.
 
# Submissions
You got a tutorial that meets the criteria above and would be useful to share? Awesome! Please reach out to us via our GitHub account. 
