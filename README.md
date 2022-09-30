## Messenger

Digital Ocean: http://165.227.253.229/

- The goal of this application is to send message to receiver. For a similar use of note, user could view the detail information of the message they choose to send and be able to edit the corresponding messege and save witht the changes. 
- The most challenge I've met is to host the application on the external site. I've tried heroku for the first time but I don't know why there's nothing shown on the site with everything built and run appropriatedly. I've tried to switched from github connection to CLI. I installed and configured the heroku CLI and tried to build a new project, with every configuration updated with running `npm install --save --save-exact`, but still nothing happened. Then I changed to ditial ocean. The application site is still having issue with the deployment. I've viewed the log and tried to fix it from the error it gave me, but things are not working as what I expected. So I changed to the droplet channel, and redo everything in the console, including the configurations. Then I had the ip address working well with `node server.js`. However, when I terminated the window, the application crashed. I've tried to do the doman things,and did a lot researches, tried _go_ _daddy_, _namecheap_. I've tried `tmux`, `screen`, and other sync methods to make everything working in background, but failed. At last, I've used pm2 to solve it. pm2 is a great application for keeping a node process running regardless of crashes, basically whenever a crash occurs it just restarts node using the same script.  
- I chose password-based authentication(OAuth) strategy which is the most common one to me. Though using passport seems to be easier, I felt like passowrd-based authentication seems to be more appropriate to my app. 
- I've used bootstrap for stylesheet since it is easy to manage and configure. The syntax could be simply found on the official lib.
- I've changed the _body_, _table_, _title_, _header_ etc. stuffs to be my assigned color and font.
- middleware
  * cookieSession - Establish cookie-based sessions.
  * body-parser - Parse HTTP request body.
  * morgan - HTTP request logger.
  * serve-favicon - Serve a favicon.
  * serve-static - Serve static files.
  
## Lighthouse Score
![100](https://media.discordapp.net/attachments/1025448793862316124/1025448875638661160/Xnip2022-09-29_05-28-54.jpg?width=1872&height=936)

## Technical Achievements
- **Tech Achievement 1**:  
 - I used OAuth authentication via the GitHub strategy
 - I host your site on Digital Ocean
 - Get 100% in all four lighthouse tests

### Design/Evaluation Achievements
- **Design Achievement 1**: 
<details>
<summary>I followed the following tips from the W3C Web Accessibility Initiative</summary>
 
 1. Provide informative, unique page titles
  * I added page tile and corresponding favicon to inform about the page
 2. Make link text meaningful
  * I made each link followed url-friendly rule and are meaninngful to lead to
 3. Provide clear instructions
  * I have instructiona and alerts for each steps/mistakes user would ever made
 4. Keep content clear and concise
  * I have everything set up clearly and organized. Codes are written with `<div>` to stay in organized paragraph
 5. Associate a label with every form control
  * Having label for every form control and placeholder for instruction
 6. Identify page language and language changes
  * I identified the page language to be English
 7. Provide sufficient contrast between foreground and background
  * I have everything in off-white, and significant colors of interactive items
 8. Ensure that interactive elements are easy to identify
  * Buttons/Inputs/Links are easy to find with placeholder/labels/captions
 9. Provide clear and consistent navigation options
  * Have nice label/instruction on every element, having alearts to guide the users if they have misoperations
 10. Ensure that form elements include clearly associated labels
  * Form has label shows the detail info and placeholder for user to take as an example
 11. Provide easily identifiable feedback
 12. Use headings and spacing to group related content
 
</details>

