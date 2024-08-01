# Le Répertoire School of Cooking
Le Répertoire is a cooking school which offers a range of classes in cooking different cuisines for students of a range of different abilities.

Users of this website will be able to find all the information they need to know about Le Répertoire including the classes offered and their schedules, pricing, a gallery of student-created food, and how to sign up for classes. The site is targetted towards people who may be interested in learning to cook, or who already have an interest in cooking but want to improve their skills.

## Features

## Design
### Design Philisophy
My aim in the visual design of the site was to reflect the elegance of fine dining. I made use of a simple greyscale colour scheme for text elements, whilst using visually striking images of food in colour to create visual interest.

The index page in particular is leans into this by presenting a full-height image of a delicious-looking plate of food, with the only other elements being a title and sub-title, along with a down arrow at the bottom of the page to help users to understand that they can scroll down to see more. I considered using content-peeking here but I really wanted to stick to the idea of keeping the image taking up the full height of the viewport.

I originally intended to leave the header / nav bar off this page which would have better fit with my design vision, but I didn't want to sacrifice usability and the ability for users to quickly and easily find the information they want. Therefore I chose to keep the header consistent across each page.

I sourced high-resolution, visually striking images from [Unsplash](https://unsplash.com/) which has a permissive license allowing both commercial and non-commercial use with no permission. I have credited the photographers in this README.

### Responsiveness
I used a mobile-first process where I developed the site first to display properly on mobile devices, and then added media queries to scale-up where needed if the mobile site did not display properly on tablet, laptop and desktop devices.

I used optimised images in a .webp format and served different-sized images to users based on the size of their display. Because of the mobile-first design, the default image served is the smallest available, and then media queries were used to serve larger images to devices with larger screens. As a general rule, for images expected to take up the whole width of the viewport (such as the index hero image), I used the following sizes:
- Small (sm) 575px wide
- Medium (md) 767px wide
- Large (lg) 1439px wide
- Extra large (xl) 1920px wide
- Original (og) original resolution to account for extremely large devices such as ultrawide monitors

## Project Management
I used GitHub projects to help me to manage the development of the site. Although I was working alone, this still made it easier to break down the development into manageable tasks, which I could prioritise and complete in a sensible order.

To further assist with prioritisation and prevent feature-creep, I broke down the project into 3 iterations and allocated each task to an iteration:
- Iteration 1 was the minimum features required to achieve at least a pass-level grade and a functional website. This included the 3 pages that I identified as being the minimum required (index, gallery and signup), as well as the README, deployment and basic testing.
- Iteration 2 included some "good to have" features such as two additional pages (a class schedule and an about page) which I felt would help me to acheive a higher grade
- Iteration 3 was where I put my "nice to have if there's time" features and tasks. These were items which I felt weren't necessary to the site working as intended and providing a great user experience, but might enhance the visual design for instance. These were mostly items which would require the use of technologies not yet covered in the course, but I do already have some experience with (such as JavaScript). These features include a filter on the gallery page, and some scroll animations on the homepage when the user clicks the down arrow. I decided that if I didn't get around to completing this iteration, I would simply add these features to my "future development" section.

The GitHub project can be accessed [here](https://github.com/users/barns/projects/3/views/4).

## Deployment
The site was deployed to GitHub pages. I deployed the site very early on in the project and then continued to deploy subsequent iterations in order to ensure that I had a working deployment in plenty of time for the deadline, and in order to test that the site worked as intended in the production environment as well as on my development server.

I set the deployment branch to `main`, and then any subsequent development was completed on a seperate branch, with a pull request only being created and merged when I was happy with the changes I had made. This reduced the chance of me accidentally pushing broken code to my production site.

I continued to use on `development` branch throughout the project because I knew that, as I was the only collaborator and was never working directly on the main branch, that branch would never fall behind `main`.

The link can be found here - [https://barns.github.io/le-repertoire/](https://barns.github.io/le-repertoire/)

## Testing

## Challenges
There were several challenges throughout the project both of a technical and non-technical nature.

One of the first issues I encountered was that, although the site displayed correctly in the responsive view of both Brave (chromium-based) and Firefox browsers, when I deployed it to GitHub Pages and viewed it on my IOS device (iPhone 11 Pro), the fixed background images' `background-attachment` property not only reverted to the default `scroll` value, but also blew up the size of the image to the point that it was pixelated and it wasn't clear what the image actually showed. From research, it appears that mobile devices do not display fixed backgrounds as it's relatively processor-intensive. Fortunately due to the early continuous deployment strategy I adopted, I noticed this very quickly and was able to address it by adding a media query to the CSS which applies to mobile devices: `@media (pointer: coarse)`, and reverts the `background-attachment` property to its initial value for the affected areas.

Another challenge that I encountered was when creating the signup form. I used checkboxes to allow users to select a number of classes (as students might be interested in several different classes, using radio buttons would not have been appropriate). I wanted to validate the form to ensure that users chose at least one class that they were interested in, but there isn't a way to do this in pure HTML with multiple checkboxes. Applying the `required` attribute to every checkbox enforces that every checkbox must be ticked, rather than at least one. The solution to this uses JavaScript, so I added a task to my iteration 3 backlog and in the meantime decided that it would be ok if some users submitted queries without selecting a class, they would just need a phone call or email to confirm which they were interested in.

## Credits

### Content
- All of the content for the site is original writing by me
- Icons used across the site are from [Font Awesome](https://fontawesome.com/)
- Code for the collapsible navbar is based on the implementation in the Code Institute walkthrough project Love Running. My deployment of that project can be found on [GitHub pages](https://barns.github.io/love-running/) and the code can be seen in [my repo](https://github.com/barns/love-running/)
- Fonts used are both from [Google Fonts](https://fonts.google.com/)
- I used the [WAVE accessibility checker](https://wave.webaim.org/) provided by WebAIM to test and improve the accessibility of my site

### Images
All images on the site are taken from Unsplash and are used under the [Unsplash license](https://unsplash.com/license). I would like to thank the following photographers for their excellent images:

- [emy](https://unsplash.com/@emysong_?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash):
  - "flat-lay photography of vegetable soup on white ceramic cup" (index page hero image)
- [Serghei Savchiuc](https://unsplash.com/@serioja?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash):
  - "a table topped with lots of pastries next to a cup of coffee" (index page)