<!-- I use this template: https://github.com/dbader/readme-template/blob/master/README.md -->
# Reddit Timer
(or How to find the best time to post your subreddit)

Use historical posts data to determine the best time to post a subreddit.

This project is the result of a course by [ooloo.io](https://ooloo.io/).
The project aims to build a professional web app with professional tools and methods.

The lead developer [Johannes](https://jkettmann.com/author/johannes/) at ooloo.io provided the project designs in [Zeplin](https://zeplin.io/) with tasks managed in [ClickUp](https://clickup.com/) management tool.
One of the requirements is that each taks be implemented within its own pull request(PR). And the PR is reviewed by the lead developer before it's merged.

Beside the project being implemented with the React library, additional tools and packages nesesary to deliver the project to plan were free to choose.
During the development process, I occasionally used TDD methodology to implement some tasks, such as header, footer, form tasks.

To ensure code quality and conformity an end to end (e2e) Cypress test suite was also provided.
I implemented the integragration tests using React Testing-Library to meet the project's acceptance criteria (AC).

The folowing are the screenshots of the different stages of the project:

![Home page](https://res.cloudinary.com/krikitue/image/upload/v1603729023/reddit-timer/homePage_rpbxun.png)
![Search page](https://res.cloudinary.com/krikitue/image/upload/v1603729024/reddit-timer/searchPage_lchzu0.png)
![Loading the data](https://res.cloudinary.com/krikitue/image/upload/v1603729496/reddit-timer/loading_ncgf0d.png)
![Display the posts](https://res.cloudinary.com/krikitue/image/upload/v1603729024/reddit-timer/posts_sgabn4.png)

## Tech Stack used:
1. **React/React Hooks**
2. **Styled-components**
3. **Cypress**
4. **React Testing-Library**

## Tools
1. [ClickUp](https://clickup.com/)
2. [Zeplin](https://zeplin.io/)
3. [Perfect Pixel](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=en)
4. **GitHub** version control repository
5. **Slack** Team communication tool

## I Proposed these Added Features
For me this is the most important part of the project where I was able to apply the knowledge learnt to propose features and deliver solutions to improve on the app.
So in addition to the original AC (acceptance criteria), I proposed and implemented the folowing features:

1. **highlights for cells** containing posts with deleted author
2. display the posts table in **modal mode to avoid the table to show below the fold**.
we could implement auto-scoll but the user would have to scroll up back to the heatmap grid again. I think offering an modal display option was practical.
3. **choose the heatmap color theme** to provide the user with another viewing comfort.
4. **make the app responsive** on all devices.
5. provide **integration and end to end tests for these features** without breaking the original AC.

## Features Solutions screenshots

1. Cell highlight to indicate it contains deleted author
![Feature #1](https://res.cloudinary.com/krikitue/image/upload/v1603729023/reddit-timer/feature_1_wnshm8.png)
2. choose the heatmap color scheme
![Feature #2](https://res.cloudinary.com/krikitue/image/upload/v1603729023/reddit-timer/feature_2_ygcnrv.png)
3. display the posts table in a modal window
![Feature #3](https://res.cloudinary.com/krikitue/image/upload/v1603729023/reddit-timer/postsModal_wy5ai7.png)
4. responsive on small screens
![Feature #4](https://res.cloudinary.com/krikitue/image/upload/v1603729023/reddit-timer/responsive_fgefov.png)
5. tests
![Feature tests](https://res.cloudinary.com/krikitue/image/upload/v1603729024/reddit-timer/tests_g26rwl.png)

## Project Highlights

- The use of [styled-components]() makes it easy to solve css issues for the heatmap color scheme.
- Tags are components offering flexibility and ease of styling
- Practical components design structure and **'DRY' coding technique** with global variables and styles used throughout the app
- Efficient successive **fetch calls using recursion**
- Effective use of **reduce functions composition** to yield complex data

- **Testing using snapshot** for the table that has 168 cells.
- **Mocks to avoid puting strain on memory**
- **Avoid data mutation on a parameter passed by reference**

## Take Away from this Project:

1. Work as Pro frontend developer using Pro methodology and Tools:
- Agile project management with ClickUp
- Slack Team collaboration platform
- E2E testing with Cypress
- Jest and React Testing-library (with hooks and mocks)
- Team linting style
2. Professional Git pull request (PR) workflow:
- pull requests (PR)
- code review
- branch merge
- branch conflicts resolution
3. Production Deployment
- Live app deployed to Netlify with CC/CI webhook
4. Apply techniques learnt to extend/improve the app UI/UX as detailed in [Features section](#I Proposed these Added Features)

## Installation

OS X & Linux:
```sh
yarn install
```
## Usage

After all the packages have been successfully installed, you can run:

```sh
yarn start
```
## Test

Run the tests with:

```sh
yarn test
```

```sh
yarn cypress:open
```
## Meta
Konan Houphoue – [@linkedIn](https://linkedIn.com/bahobab) – khoophdev@gmail.com
[https://github.com/bahobab](https://github.com/bahobab/)

<!-- ## Contributing

1. Fork it (<https://github.com/yourname/yourproject/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request -->