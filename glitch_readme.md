# Welcome to StudioBot!

StudioBot interacts with students and professors primarily through conversation and simple graphical interfaces such as buttons. The bot has two modes of interaction with users: responses and performances.

When the bot responds to a user, it is usually being asked for information (which it will supply if it is available) or mentioned in conversation. This mode of interaction gives a wide degree of freedom to the path of the conversation, which is usually an informal chat. This is essentially the functionality of a chat-bot, except it will also have access to many studio resources that it can relay to the students on Slack. This allows information to be distributed as it is needed, and searchable within Slack (as well as re-queryable).

However, answering questions and responding to a flurry of informal chats is not StudioBot's primary function. This bot is designed to perform actions and complete tasks that facilitate studio engagement as well as to provide tools for students and professors that both simplifies their workflow and amplifies their productivity.

## Modes of Interaction

#### Basic Response Interactions
##### Common
* **hello**: *A simple hello script that displays a random greeting each time someone says hello to it*
* **goodbye**: *A simple goodbye script that displays a random farewell each time someone says goodbye to it*
* **identify**: *Responds with its identity, what it does (in simple terms) and asks if you would like to see the help command*
* **channel_join**: *Response to being added/invited to a channel. Gives a few unobtrusive hints to it's most useful features*
##### Studio
* **syllabus**: *Responds with a link with the syllabus attached. Might shoot a sassy comment*

#### Basic Performance Interactions
##### Common
* **create_profile**: *Walks the user through the creation of a profile that will be persisted to a database for reference in the future*
* **onboarding**: *Welcomes a new user to the studio*
* **check_in**: *Bot checks in once a week (probably a Friday) to monitor students' stress and outlook. Will persist student responses to database for analysis, and reply with uplifting of motivating responses*

#### Complex Response Interactions
##### Common
* **help**: *Will respond with a short message containing a few of the most useful commands, and will ask if the user would like to see help for all commands. Also accepts an argument containing the name of the specific command the user would like to see help for*
* **thanks**: *Responds with a random "you're welcome" message, and asks if the user would like assistance with anything else. If yes, and user added what they wanted done, do task. If yes, and user hasn't included what they want done, ask. If no, end thread*
* **status**: *If a crit session has been launched (and not closed), StudioBot responds with a percentage bar showing how far along the professor is and how much time remains until users crit. If a crit session has not been launched, or has been closed, StudioBot responds with a message saying a crit session has not been launched or has been closed. If the day is not a studio day, .*
* **deliverables**: *Will reply with the deliverables that were set during the set-deliverables command*

#### Complex Performance Interactions
##### Studio
* **launch-crit**: *Launches an interactive prompt to everyone in the studio asking which position they would like to sign up to for desk crits that day. As students begin selecting their positions, the prompt dynamically changes to reflect the students position. If a students response times out, and they don't respond to the follow-up message, they will be appended to the end of the order. StudioBot then equally allocates time to each student for their desk-crit within studio hours. StudioBot also sends private messages to each student 2 minutes before their crit, and notifies the professor when it is time to move on. launch-crit is automatically launched every Mon, Wed, and Thurs at 1:30pm, but it can be launched manually on any day with a different number of students or amount of time*
`@StudioBot launch-crit start end n_students`
`@StudioBot launch-crit 10:00 14:00 13`
* **set-deliverables**: *Will ask user to send a multi-line message containing the deliverables for the week, studio, or pinup*








lunchtrain?
