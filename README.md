# CosCalendar - Cosplay Planning App

![am-i-responsive-_1](https://github.com/emmy-codes/coscalendar/assets/70635859/ffc2e943-c4ad-4eaa-aadb-9489556fe87f)


This is my 5th and final project at Code Institute, implementing all skills learned so far and focusing on an output using React on the frontend and Django REST API on the backend. This project is designed with cosplayers in mind, to help them stay accountable for their cosplay plans by tracking their project plans in a calendar, as well as the costs accrued whilst crafting the cosplay. This gives the cosplayer a detailed overview of time management and expenses for their projects.

The full plan for the website is listed below under "Features".

Link to live API on Heroku: https://coscalendar-api-3bdc9b15f518.herokuapp.com/

Link to live site on Heroku: https://coscalendar-495a347f9b5a.herokuapp.com/

----------

## CONTENTS

* [User Stories](#user-stories)

* [Design](#design)
	* [Accessibility](#accessibility)
  * [Wireframes](#wireframes)

* [Features](#features)

* [Technologies Used](#technologies-used)
	* [Languages Used](#languages-used)
	* [Frameworks, Libraries & Programs Used](#frameworks-libraries--programs-used)

* [Iteration over starting code](#iteration-over-starting-code)

* [Deployment & Local Development](#deployment--local-development)
	* [Deployment](#deployment)
	* [Local Development](#local-development)
	* [How to Fork](#how-to-fork)
	* [How to Clone](#how-to-clone)

* [Testing](#testing)

* [Bug Fixes](#bug-fixes)
  
* [Plans vs Execution](#plans-vs-execution)

* [Code Used](#code-used)

* [Content](#content)

* [Acknowledgments](#acknowledgments)

- - - 

## User Stories

| Epic | User Story  |
|--------------|---|
| All Users | As a User, I wish to view the landing page so I can see the available content  |  
|              | As a User, I wish to click on the nav bar links so I can navigate to the selected content   |
|              | As a User, I wish to navigate the selected content quickly so I can view content without page refresh |
|              | As a User, I wish to see my profile link in order to easily tell if I'm logged in or not |
|       (not MVP)    | As a User, I wish to browse the current list of user-added conventions so I can see if my desired convention already exists |
| Unauthenticated User | As an Unauthenticated User, I wish to register an account by clicking Register so I can make use of the authenticated user content | 
|              | As an Unauthenticated User, I wish to click login so I can access certain features  | 
|              | As an Unauthenticated User, I wish to receive descriptive error messages so I can tell if my registration or login has failed | 
| Authenticated User | As an Authenticated User I wish to Sign out of the website so that my profile can remain safe when I want it to | 
|              | As an Authenticated User, I wish to make a cosplay to-do item on the calendar so I can plan and mark off steps to complete my cosplay   |
|              | As an Authenticated User, I wish to view my cosplay to-do item so I have an overview of the task  |
|              |  As an Authenticated User, I wish to add notes to my cosplay plans so I can put down thoughts outside of the to-do checklist  |
|    (not MVP)   | As an Authenticated User, I wish to add a convention so I can enable other users to find it and/or add my own cosplay plans to the convention |
|    (not MVP)  | As an Authenticated User, I wish to save a convention to my profile so I can keep track of events I'm interested in  |  
|              | As an Authenticated User, I wish to mark tasks on my to-do list as complete, so I can track my progress   |
|              |  As an Authenticated User I wish to update my username and/or password in order to change my name if I wish and/or ensure my account is safe  |
|              | As an Authenticated User I wish to add a profile picture in order to customize my profile   |
|              | As an Authenticated User I wish to edit a profile picture in order to update my picture when I want to  |
|              | As an Authenticated User I wish to delete a profile picture in order to remove my cosplay from the internet if I wish  |
|              | As an Authenticated User I wish to add expenses for a selected cosplay so I can track costs for the project |
|              | As an Authenticated User, I wish to be able to edit or delete expenses so I can control the costs I am tracking |
|   Site Admin  | As a Site Admin I wish to delete user's content if necessary so I can control the sort of content on the site  | 
|              | As a Site Admin I wish to view the admin dashboard so I can review the site metrics (to see how many users are using cosplans, expenses etc)   |
  

- - -

## Design

The design is going to be simple to avoid too much time being spent on superficial things as I am still very keen on practicing my backend skills. The page will be clear and concise to keep the user's focus on the functionality, the planning part of the page.

I wanted some calming blue tones but came across a colour palette that has a mixture of purple and blue with turquoise and green. Purple is said to symbolize, among others, creativity and peace, which I felt fit in with my plan:

![coolors_palette](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/57ea61ee-75b7-456e-97d4-466aa5016012)

### Accessibility

Any imagery will be addressed using alt tags, and the above colour palette has very minimal variation in Coolor's colour blindness comparison! Semantic HTML will be used wherever React components aren't being rendered, and those components will have clear names to specify their use (although I know they'll be converted into JS and HTML in the browser).

### Wireframes
Below I have added the comparison of wireframe vs live site to effectively prove that I followed the plans through to completion. I think they came out looking very similar to the original sketches! I didn't have the Expenses in mind originally so I did wing that design based off the Tailwind components so there was no wireframe planned for that and I didn't have time to fix one retroactively.

Homepage/login: The homepage is going to go straight to offering to login/sign up - After coding: I wanted more than just an introduction to the page beside the login info, so I added a simple homepage to help users understand the uses of the site.

![login_wireframes](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/85ef6063-e9f2-46df-9d29-47b9162fd551)

![homepage_desktop](https://github.com/emmy-codes/coscalendar-api/assets/70635859/77ae2495-3d1a-4b65-b742-8f1540faa2d3)
![homepage_mobile](https://github.com/emmy-codes/coscalendar-api/assets/70635859/94d9b7da-d1d2-4417-baab-f21c7b9c63a5)
![homepage_tablet](https://github.com/emmy-codes/coscalendar-api/assets/70635859/577cc4f0-06c3-4824-b413-257d678d5e58)
![login_desktop](https://github.com/emmy-codes/coscalendar-api/assets/70635859/6566a4e5-d746-4731-89cf-3b4392f880b0)
![login_mobile](https://github.com/emmy-codes/coscalendar-api/assets/70635859/e9776673-43d2-4cfd-b71d-6bc333ad03ec)
![login_tablet](https://github.com/emmy-codes/coscalendar-api/assets/70635859/72c6dfad-e617-4934-967f-04d2b6d41749)

Register: 

![register_wireframes](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/030b2f00-27b4-4347-815d-6243e86a6f33)
![desktop_register](https://github.com/emmy-codes/coscalendar/assets/70635859/552ae0c7-d9b1-4237-98f5-cf30613907a0)
![register_tablet](https://github.com/emmy-codes/coscalendar-api/assets/70635859/bd5d70ed-f97b-4732-823e-c7b55d8348bb)
![register_mobile](https://github.com/emmy-codes/coscalendar-api/assets/70635859/b587a358-c1c2-4ee1-bb06-97fa50eeeee1)


CosCalendar:

![calendar_wireframe](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/ef2f850f-3cc3-4d85-8406-9bdc3e74433e)
![coscalendar_desktop](https://github.com/emmy-codes/coscalendar-api/assets/70635859/08f2b19b-36df-4379-a8ad-353155529573)
![coscalendar_tablet](https://github.com/emmy-codes/coscalendar-api/assets/70635859/ff5c3cad-b6ab-4708-967b-3f371e1319ae)
![coscalendar_mobile](https://github.com/emmy-codes/coscalendar-api/assets/70635859/270c2ce4-7dfb-410f-b176-742cd4dea2c7)


Add cosplan popup: When the user edits one of their plans the same window will popup, so this serves both as add new and edit existing plans - After coding: The popup was a good idea but I went with a separate page to help me to execute the plan effectively with the knowledge I had of data rendering and redirection/navigation.

![add_plan_popup_wireframe](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/a0cd2ffc-bcb8-498a-9019-9d5a16f5aa16)
![cosplanform_desktop](https://github.com/emmy-codes/coscalendar-api/assets/70635859/437af48f-e61a-46b7-b753-1ed06ca51281)
![cosplanform_tablet](https://github.com/emmy-codes/coscalendar-api/assets/70635859/7363743c-e6bf-4031-a1a3-84c42eff7756)
![cosplanform_mobile](https://github.com/emmy-codes/coscalendar/assets/70635859/f6d4a5b3-4aeb-49f1-a771-078d3dfb52b4)

Expenses (no wireframe):
![expenses_desktop](https://github.com/emmy-codes/coscalendar/assets/70635859/6dcf0339-c8b5-43f7-9406-569623465f85)
![expenses_tablet](https://github.com/emmy-codes/coscalendar/assets/70635859/81790048-68ea-4184-92fd-0b83eca3015c)
![expenses_mobile](https://github.com/emmy-codes/coscalendar/assets/70635859/f4750194-8121-4cda-97a9-2913044a4d80)



## Features

I am planning a cosplay planning page for cosplayers to help them stay accountable when con crunching (a phrase often used in the community for panicking to make your cosplay in time).

An unathenticated user will be encouraged to log in/sign up to access the content.

An authenticated user will have a profile of their basic information. Uncertain if there will be further functionaliy here yet.

The main page will be a calendar type app but with a larger list of events to the side of/underneath the calendar. This will be the cosplayers' plans to stay on top of and they won't have to click on a specific date to see the plans. This way the focus is more on the to-do list aspect of the planning than just looking like an imitation Google Calendar.

It would be nice to have them coloured in order of date - any within a week of the convention are red, from there and up to a month before the convention are yellow, then green or so. This would help the cosplayer at a glance to see how many items are left on their planning app.

On the overview cosplayers will be able to go delete the to-do action, as well as click on it for further information.

In the task overview page there an editable text pre-filled with the user's to-do information. The user can save the updated information (such as changing the date or adding/removing text details).

It will also be possible to click on a date to add a task which will bring the user to the same page as the edit task, but with no data pulled from the database.

There will also be a section that acts as an expenses tracker/shopping list, where cosplayers will create/select one of their cosplay characters, and from there they can add items that they need to purchase or items they have bought during the creation of their cosplay. 

In each item the user can add/update/remove the following: 

- Name of the item to purchase/already bought
- Item cost (per item)
- Maybe amount (ie 2x red paint)
- Optional link to the item to buy/bought
- Total cost of all items added

This is to help the cosplayer track the expenses included in each cosplan they have.

- - - 

## Technologies Used

### Languages Used
 
HTML
CSS
JavaScript
Python
Tailwind CSS and components

### Frameworks, Libraries & Programs Used

[Github](https://github.com/) - For online storage of code and deployment.

[Picresize](https://picresize.com/) - Used to resize images for Readme/Testing docs.

[VS Code](https://code.visualstudio.com/) - For writing my code.

[Heroku](https://dashboard.heroku.com/apps) - For deploying my program.

[Grammarly](https://app.grammarly.com/) - For grammatical adjustments.

[Materialize](https://materializecss.com/) - Framework to make responsive front-end solutions.

[Django](https://www.djangoproject.com/) - To build my CRUD functionality.

[PostgreSQL](https://www.postgresql.org/) - For my Database.

[Cloudinary](https://cloudinary.com/) - For hosting blog images.

[Coolors](https://coolors.co/) - To create colour palettes.

[Tailwind CSS color generator](https://uicolors.app/) - To generate a CSS palette for Tailwind.

[React](https://react.dev/) - For organising/structuring the code.

[Pexels](https://www.pexels.com/) - For free images for the site.

- - -
  

## Iteration over starting code

The first iteration was done using 3 Tailwind UI React components which was quick to give the page a decent structure out of the box.

The calendar is the meat and veg of this page and much of the premade component data is static so will be needing a lot of refactoring. There's so much functionality involved in a calendar app that I decided to use the date-fn library to help me piece it all together.

Premade date-fn functions:

[startOfDay](https://date-fns.org/v3.6.0/docs/startOfDay) - Returns the start of a day.

[startOfWeek](https://date-fns.org/v3.6.0/docs/startOfWeek) - Returns the start of the week for the given date.

[endOfMonth](https://date-fns.org/v3.6.0/docs/endOfMonth) - Returns the end of a month for the given date.

[endOfWeek](https://date-fns.org/v3.6.0/docs/endOfWeek) - Returns the end of a week for the given date.

[eachDayOfInterval](https://date-fns.org/v3.6.0/docs/eachDayOfInterval) - Returns the array of dates within a specified time interval.


In my code these do the following:

1. The function getCalendarMonth uses the variable todaysDate which returns todays date using startOfDay
2. The firstCalendarDay variable calculates the start of the week from todaysDate
3. The lastDayOfMonth variable calculates the last day of the month (which isn’t the last date, as it could be that the beginning of the next month is in the middle of the week)
4. The lastCalendarDay variable calculates the final day in the calendar’s month overview by finding the endOfWeek of the lastDayOfMonth
5. Then returns eachDayOfInterval that receives the start and the end as the first and last days of the weeks in the monthly calendar view

That’s a lot of going backwards between the variables! But I was then able to replace the premade render with getCalendarMonth() which continued to map over the data as before.


- - -

## Deployment & Local Development

### Deployment

This project was deployed at [Heroku](https://heroku.com/)

The numbers on the screenshots represent the numbers on the steps of my deployment process.

To deploy this project after creating my account, I:

1. Went to my dashboard and clicked on the New App dropdown menu

2. Clicked Create new app from the options
  

![heroku_deployment_step_1-2](https://github.com/emmy-codes/cat-adventures-python/assets/70635859/f5810840-3399-48aa-8944-384850e2f6d9)


3. Named my app in the App name box

4. Chose a region from the dropdown menu (and accidentally chose the United States for this one)

5. Clicked Create app


![heroku_deployment_step_2-5](https://github.com/emmy-codes/cat-adventures-python/assets/70635859/be20a348-416c-446c-8876-2a33ccb883bb)

Once the app was made I went to my dashboard where I can see my apps.

6. Clicked on the relevant app

![deployment-step-6](https://github.com/emmy-codes/coscalendar/assets/70635859/44d2a777-fc16-43ea-8b73-4a731a7378be)

7. Under the Deploy tab, I connected my Github repo to the Deployment method

![deploy-step-7](https://github.com/emmy-codes/coscalendar/assets/70635859/479a87da-628b-44f9-80b9-8a192d007fdf)

8. Adding buildpacks: Click on the Add buildpack button, select nodejs from the supported buildpacks, and Add Buildpack. This will allow Heroku to deploy successfully.

![deploy-step-8](https://github.com/emmy-codes/coscalendar/assets/70635859/a2277585-e160-41e4-906c-fb0fca3e25f1)

9. Scrolling down the page, I chose which branch to deploy, and then manually deployed my project, but it's possible to set up automatic deployments if preferred.

![deploy-step-8](https://github.com/emmy-codes/coscalendar/assets/70635859/97582426-0d13-4c14-9570-0617ecf5efcb)

### Local Development


#### How to Fork


Should you wish to fork this repo, here is a guide on how to do that:


Firstly, go to https://github.com/emmy-codes/coscalendar/


1. On the main repo page, click the Fork button near the top right corner
![fork1](https://github.com/emmy-codes/coscalendar/assets/70635859/8d04dda9-21d4-4623-9b59-4f16736f3329)


2. On the create a fork page, check the Owner of the repo is set to the GitHub org you wish to use, and change the name of the repo if you wish.

	2a: Add a description if you want to.

3. Check the box here if you want to make a copy of the main branch or multiple branches (main is selected by default).

4. Create the fork. The screenshot is from an old project as I cannot fork my project due to not having any organizations connected to my account any longer.
 
 ![rsz_fork__steps](https://github.com/emmy-codes/geekhaven-blog/assets/70635859/aa4dae7c-807d-4108-bb5b-f24c7010514b)


#### How to Clone
  

For cloning the repo you will need:

* The [repo](https://github.com/emmy-codes/coscalendar) open
 

* Your IDE of choice

1. On the repo page, click on the green "Code" button

2. On the dropdown from the Code button, click on your chosen key (pictured here is SSH)

3. Click the copy button (shown as two squares on top of one another) 

![fork2](https://github.com/emmy-codes/coscalendar/assets/70635859/a37aea8e-46f9-4b68-8bf3-af57c402af16)


4. Open your IDE of choice and open the Terminal, or in my case, open the Terminal on your computer (I run Linux on Windows so may be slightly different for Mac/Windows users)

5. Check that you're in the right folder (shown here by checking my current folder by using the input: ls

6. Change as needed to reach your desired folder.

7. Type (without quotation marks): "git clone" followed by your copied link from GitHub.
  
![fork3](https://github.com/emmy-codes/coscalendar/assets/70635859/f3547538-397b-4d64-a63e-b74364e4019d)

8. You can now access the repo in your IDE if cloned directly there, or by typing (without quotation marks) "code ." in your Terminal.

9. Enjoy! 

- - -
  

## Testing

Please refer to the [TESTING.md](https://github.com/emmy-codes/coscalendar/blob/main/TESTING.md) file for manual testing and screenshots.

## Bug Fixes

1. Once I added the functionality to correctly track the monthly calendar days/weeks, the render was a huge mess!

![calendar_visual_bug1](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/14866dc4-0543-4fdb-aa84-11ca54cb411c)

I first inspected the calendar grid in Chrome dev tools and could see that it was rendering the dates I had just coded, so I added a console.log using the "day" parameter. This gave me a full log of the dates that I expected for this month, so at least the functionality was working but the render wasn't.

![calendar_visual_bug2](https://github.com/emmy-codes/CosCalendar-cosplay-planning-page/assets/70635859/b6c10991-10f4-47d3-9029-fd7088fdc904)

This looked like it was correct since the dates themselves were correctly rendering. It wasn't until 3 days later when I was discussing the problem with my partner and he asked to see the log, then pointed out that it's literally rendering from the date, the time, GMT timezone etc, all trying to squeeze into the tiny grid block for each date. All that text when I just wanted Day, Month, Date!

So back to the documentation, I went looking to complete my logic for accessing the right content. I looked over my date-fn functions and noticed I had endOfMonth, but I should need startOfMonth to get the beginning of the calendar, right? Currently my calendar was rendering from today's date and onwards.

After further research through the date-fn documentation I came across mention of Unicode Tokens and discovered that DD refers to the day of the year, whereas dd refers to the day of the month, which is why in the case of my calendar it's important to use lowercase letters. [source](https://github.com/date-fns/date-fns/blob/main/docs/unicodeTokens.md)

Seeing as the component is pre-built I had to do some research into its contents. I'd never come across the <time> tag before so upon reading up on [MDN documents](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time) I learned that the dateTime attribute allows us to set specific day/time values inside of the tag, to me that seems somewhat like how we add attributes to forms!

I decided to pass my formatDates variable to both the dateTime attribute, and the render inside the time tag. Viola! I was no longer rendering a huge mess of data and my calendar was readable! The wrong month, but readable. I'm still not entirely certain why we provide the dateTime value inside if it's also being rendered within the tag itsself, but at least it was working. From what I've read, it is for the benefit of the machines and for search engines, but I'll leave it at that for now.

2. Tailwind CSS vs global CSS variables: I wanted to use global variables for readability, and ease of updating in the future. It worked well to have the variables under :root, and when I changed the background of a div it worked, but trying to use the Tailwind CSS component text-<colour>-<weight> with a variable didn't do anything.

Doing research on the matter, I discovered that, due to the way Tailwind processes the classes, and with having multiple classes with seimilar names (ie text-lg is for the size and text-black is for the colour) it struggles to define which is which on a global variable. If I, for example, tried to have a hexcode under the variable name --textColor and then used the className on my HTML for trying to style the text: text-[var(--textColor)] it doesn't know if that's a CSS for text COLOUR or SIZE, and thus does nothing.

There was [some documentation](https://tailwindcss.com/docs/adding-custom-styles#resolving-ambiguities) on workarounds but it would have been more work to maintain and less user friendly if someone else or future me should look at the code.

Solution:  I dug my way through to the [TailwindCSS documentation](https://tailwindcss.com/docs/customizing-colors) which shows how to use themes which act a lot like global variables, which seemed like the least invasive and easiest solution. There is an issue with this in that using cusom colours completely overrides all of the Tailwind CSS colours, but at the beginning of my project this is a workable solution. Once my colour palette has been tested on the site I may stick to the out of the box colours from Tailwind.

![bug2-tailwind-global-variables](https://github.com/emmy-codes/coscalendar/assets/70635859/9c2e01b3-e739-4e03-b14f-6610259eb0ee)

3. I was working to create my first handleSubmit function (as I'm not using Bootstrap I could not follow the Moments walkthrough very well, so I was using resources such as [React Dev](https://react.dev/learn/updating-objects-in-state) and [MDN response OK docs](https://developer.mozilla.org/en-US/docs/Web/API/Response/ok) to help me write the state updates and the following redirects.

I originally set my if statement to use (response.ok) thinking that this would cover the successful status codes. What it did was give me this adorable error (sadly no cats showed up in the terminal though) ![httpcats204error](https://github.com/emmy-codes/coscalendar/assets/70635859/e11ade3f-2ee4-4953-8503-ce91e360e00a) reading up on it, this meant that the registration itsself was successful but that my redirect wasn't happening.

After some [more digging](https://stackoverflow.com/questions/64317691/is-there-a-less-hard-coded-alternative-to-using-if-response-status-201) I determined that since I am very specifically looking for the 201 - created http response I would add it explicitly in place of the response.ok, as well as the 204 response to prevent the function from not redirecting.

![bug3_solve](https://github.com/emmy-codes/coscalendar/assets/70635859/6511404d-7efb-4c1f-8102-9c4d1916c160)

That small change was all it took for the final piece in the functionality to work!

4. ![bug date format](https://github.com/emmy-codes/coscalendar/assets/70635859/459dc1f0-789e-4465-a24f-630c160b5c74) whilst trying to set up my POST request on my CosPlanForm component, I encountered the above error.

I thought I had correctly formatted my date details on the frontend by selecting date-fn’s formatting of my preference which was dd-MM-yyy. I did [some research](https://stackoverflow.com/questions/30798906/the-specified-value-does-not-conform-to-the-required-format-yyyy-mm-dd) and discovered that this was because Django is set to receive the yyyy-MM-dd format.

I then had a look on how to change the [default Django format](https://stackoverflow.com/questions/7737146/how-can-i-change-the-default-django-date-template-format) but after going to the [Django Docs](https://docs.djangoproject.com/en/5.0/ref/templates/builtins/#date) but this solution wasn’t going to work for my React frontend as it is only valid for Django templates.

[Further down the rabbit hole](https://stackoverflow.com/questions/7737146/how-can-i-change-the-default-django-date-template-format) I found someone with a solution to set DATE_FORMAT in my settings.py and also to use something called USE_L10N = False. Use Lion, I thought? Let’s google that. [Oh, it’s deprecated](https://stackoverflow.com/questions/77654801/use-l10n-deprecated-but-it-disables-datetime-input-formats-when-removed) .... Oh but only if you’re using Django 5 does that matter! Finally a good result from not having the most updated version of something (insert happy dance here) so I went back to update my settings with the suggested info:

![bug_date_format_django_settings](https://github.com/emmy-codes/coscalendar/assets/70635859/ab6e2e69-3e49-493f-8ebb-2f7f8e8f7ae7)

But on my frontend it was showing the format rather than the date from the Calendar select! 

![bug date format frontend borked](https://github.com/emmy-codes/coscalendar/assets/70635859/8aea94c0-e320-4dbe-a34f-042b432edf1b)

I went back to the [date-fns documentation](https://date-fns.org/v3.6.0/docs/format) and had a look at their formatting guides. I then decided I needed to try adding something similar to theirs, but I didn’t need to manually specify a date the way their examples did since I was fetching the date in my initialDueDate variable.

The frontend was now nicely showing the date that was selected on the Calendar, hurrah! And yet, upon submit...

![bug_date_format_frontend_fine_but_persistent_error](https://github.com/emmy-codes/coscalendar/assets/70635859/a3debda9-ff60-4c68-9874-ed24036972a1)

[more researching](https://docs.djangoproject.com/en/5.0/ref/settings/) uncovered that DATE_FORMAT is how Django will display the dates, but DATE_INPUT_FORMATS is what you set Django up to RECEIVE! Key there, I think.

In my settings.py I already had referenced the DATETIME_FORMAT which was different to the dd-mm-yyyy which I had intended from my frontend. I changed that, and added both DATE_FORMAT and DATE_INPUT_FORMATS to the settings to try to accept different formats, and ensure the dates are displayed as I wanted.

WRONG.

All hail our console.log overlords! It was time to see what was actually being sent or received by my POST request. I used extra console logs in the beginning to see what was being sent to the backend, and to see what response came back. (logs 1 & 2 on the screenshot). The console.error logs were there from the beginning and I had previously received a console.error in the catch part of the code, but had been focusing too hard on the date format error to look into it.

![bug_date_format_console_logging_across_the_universe](https://github.com/emmy-codes/coscalendar/assets/70635859/2d3a5683-ca53-4416-95a2-59db61e5178c)

Interesting, the “form submitted” log number 1 was showing the due_date with a totally different format than even my frontend or backend was intending to send/receive:

![bug_date_format_console_log_shows_interesting_due_date_data](https://github.com/emmy-codes/coscalendar/assets/70635859/8c1b895a-6720-4c9e-ad1b-34fdf419fadf)

This was confusing when on my Calendar.jsx I had already used the date-fn format method to ensure everything was set to dd-MM-yyyy and this was being passed to my CosPlanForm.jsx through the state object in my Link tag. I thought this would be enough to ensure that the date being used in the CosPlanForm was in the same format as my Calendar setup.
Feeling like I was low on options, despite not wanting to repeat code, I tried explicitly formatting the date within the CosPlanForm component. I also explicitly referred to the formattedDate by instead of passing the destructured cosplay variable to my post request, sending an object with all of the fields with the due_date referring to the formattedDueDate.

![bug_date_format_explicit_post_request](https://github.com/emmy-codes/coscalendar/assets/70635859/a3170f47-e01a-493d-b315-fcb19bfd6f85)

![bug date format formatting attempt on cosplanform](https://github.com/emmy-codes/coscalendar/assets/70635859/f9490cf1-30d0-46af-ae3d-e55265a5294e)

A miracle happened… I double checked my backend to ensure these were being created, and they were!!!

![bug_date_format_miracle](https://github.com/emmy-codes/coscalendar/assets/70635859/72dd05c6-647f-4660-a9ed-ca05230d8f93)

Biggest learning from this very extensive issue? Date formatting does not perpetuate between components, even when being passed as state.

# Plans vs execution
## Plans vs execution - and the things I've learned along the way - (Retro)

I believed that I had a solid plan for this project - follow the CI guide as far as possible, whilst adding my own functionality. I thought the Calendar app option was nice because it'd be different from the sea of blog pages and, as someone who prefers React over Django, I thought it was a great option for me to work on. I VASTLY underestimated the amount of coding logic involved in a Calendar, eventually having to resort to outside help to complete the setup! But once the main logic was in place I was able to stay on top of the future changes.

Overall I'm *extremely* happy with the result, it does everything I hoped it would do! But I definitely needed more time for implementation of code. Nearly every corner had a new error behind it, which took a lot of time to fix rather than working on the projects' completion. But hey, since that's dev life in the real world, it's all good learnings!

I'm not happy however with the strucutre I used in React. I know enough about it to know that there are ways to extensively improve the use of DRY method throughout the codebase, as much of my code was repetitive in each component. But lack of knowledge and time caused me to work reactively (no pun intended) rather than proactively in this matter. It's something I can definitely work on next time I work with React.

The only tickets left in my Project/Issues were either one documented bug, or features I had in mind with my original plan for this project that was quickly scrapped but I wanted to keep a record of my journey, and who knows, it may be implemented one day in the future!

Wireframing - I had a solid foundation on the wireframing, having learned from 4 previous projects and with the added knowledge of Tailwind CSS Components I had a good idea on what things would look like, and I could then tailor them using the components.

Design - I never really had a specific colour theme in mind with this project, and I just hoped that it would become clear as the project developed. The initial blue colour theme was designed with [colour psychology](https://londonimageinstitute.com/how-to-empower-yourself-with-color-psychology/) in mind. I felt the palette to be lacking though so it needed sprucing up from my original plan.

I added a few more colour themes to the Tailwind config, as well as a nice gradient background which allowed me to utilise a broader colour theme and spice the site up a bit. The blue colour was a bit Facebook-y, but I still like the colours!

Accessibility - The accessibility standard was planned here, with the use of alt text, being mindful of colour palettes so that text remains easy to read, and so forth. I received the added bonus of learning about a clever class via the Tailwind CSS components titled "sr-only" which allows for elements to be hidden on a page, but keep them accessible for screen readers. This helped to improve the accessibility of my page in ways I hadn't previously considered when we hide things that may be meaningful for visually impaired users.

Features -

1. I had originally set up my backend to contain a CosPlan table that would allow for users to select a cosplay from a dropdown menu, meaning that even though the website wasn't interactive with other users, any time a user made a reference to a specific cosplay character it'd be saved and other users could select it from a dropdown list. It never quite sat right with me but I had to roll with the idea through the project until I came to actually implementing the idea and when putting together my post requests for creating a CosPlan, I realised all I wanted on my frontend was a box for the plan and a box for the description (along with the due date but that was being handled on the Calendar page). This idea is going to be downsized to match my frontend requirements, but I will be restructuring the Expenses page as well beacuse this was originally going to be connected to a CosPlan via the cosplay reference from my models. We will see.

2. Calendar/CosPlanForm - I decided to remove the date picker from the CosPlanForm.jsx file. It would have been a nice UX to have continuation from the Calendar page so that the user could still select a date once they were starting their CosPlan, but I just found myself getting stressed out about deadlines and repeating the huge amount of code that went into the Calendar, that I swapped that for a static display of the date they selected from the Calendar page. If a user wanted to change dates, they could cancel and go back to the Calendar. It wasn’t what I wanted for the users, but I decided this timesave was worth the impact on overall UX.

3. I had not originally planned for the expenses tab but after speaking to my mentor I realised it was necessary to have another model to fulfil the LO of P5. I found the easiest way to implement it was to attach it to a created CosPlan so that users can add expenses/shopping lists for themselves. It's easy to go "Oh I need more paint!" but now they can attach that to the plan and keep a reminder to buy it. The plans I had for the name, item cost, amount, and optional link as well as the total cost were all implemented successfully.

4.  There was not a huge plan for the profile itsself, as my site was unlike the walkthrough from CI and not reliant on other users accessing it. This could be a future implementation of course, but would require a lot of refactoring. So a simple page sufficed.
5.  My plan to colour coordinate the cosplans by closeness to the due date was a nice idea, but didn't come to fruition. It feels OK though as the user can see cosplans by day rather than a huge overview as I had originally planned.
6.  There was no need to implement the ability to click the cosplan for further info, it was already rendering everything on my Calendar view :) but full CRUD functionality on the plan is there.

- - -

### Code Used

* Tailwind UI Components (Bootstrap replacement)
* Calendar - I had several mob sessions with an experienced developer who had fairly recently made a calendar for their own app and helped me to fulfil much of the base functionality (first commit of Calendar) from there on the changes were my own

### Content

Currently no large detail of content needed.  

### Acknowledgments

I would like to acknowledge the following people:

* Community Sweden - ❤️ you guys keep me going!
* Specifically Jonathan for his indepth knowledge trying to help me update my Pip and Python versions(sorry I made you into an Ubuntu fan!)
* My hubby and adorable toddler for smiling when I couldn't
* My friends and family for their support

As always, my partner for helping me
  

