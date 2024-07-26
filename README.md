# Le Répertoire School of Cooking
Le Répertoire is a cooking school which offers a range of classes in cooking different cuisines for students of a range of different abilities.

Users of this website will be able to find all the information they need to know about Le Répertoire including the classes offered and their schedules, pricing, a gallery of student-created food, and how to sign up for classes. The site is targetted towards people who may be interested in learning to cook, or who already have an interest in cooking but want to improve their skills.

## Features

## Design
### Design Philisophy
My aim in the visual design of the site was to reflect the elegance of fine dining. I made use of a simple greyscale colour scheme for text elements, whilst using visually striking images of food in colour to create visual interest.

The index page in particular is leans into this by presenting a full-height image of a delicious-looking plate of food, with the only other elements being a title and sub-title, along with a down arrow at the bottom of the page to help users to understand that they can scroll down to see more. I considered using content-peeking here but I really wanted to stick to the idea of keeping the image taking up the full height of the viewport.

I also chose to leave the header / nav bar off this page which sacrifices a small amount of user navigation in order to better fit with the visual design I desired. The user is still able to easily find the information that they need as the elements below this image provide links to all of the available pages.

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

## Credits

### Images
All images on the site are taken from Unsplash and are used under the [Unsplash license](https://unsplash.com/license). I would like to thank the following photographers for their excellent images:

- [emy](https://unsplash.com/@emysong_?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash):
  - "flat-lay photography of vegetable soup on white ceramic cup" (index page hero image)
- [Serghei Savchiuc](https://unsplash.com/@serioja?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash):
  - "a table topped with lots of pastries next to a cup of coffee" (index page)