# bagels-bikes.github.io

## Maintaining

Hello future BAGELS-BIKES website maintainer! I hope you're doing well. Here's a rundown about how to add future talks and whatnot.

0. (First time only) __Setup__. Make sure you have git installed, and then run 

```bash
git clone git@github.com:bagels-bikes/bagels-bikes.github.io.git
```
in the terminal, in whichever folder you want to keep your personal copy of the website (which you will update on your machine, and eventually upload back to github so it appears online).

1. __Updating__. First run `git pull` to make sure you're up to date. Then, edit 
- `src/bagels/bagels.json` OR
- `src/bikes/bikes.json`,

adding semesters and talks as you deem necessary. I'm following the convention that the newest semesters/talks appear at the top, and older ones down below. These are JSON files, you can look up how they are structured, or you can try to mimic the pattern that's already there with the existing talks.

2. (Optional) __Test locally__. You need to install `node` (with npm) over [here](https://nodejs.org/en/download/current), though be warned that installing on Windows is a little complicated nowadays. This isn't the recommended way, but it's definitely easier to follow the "Or get a prebuilt Node.js® for..." and getting the Windows installer (the .msi file). Then, once you have node installed, run `npm install` inside the project folder, and then `npm run start`. You should then be able to go to [http://localhost:8080/](http://localhost:8080/) and test out your changes.

3. __Push your changes__ to the internet. Run
- `git add .` to make git track all the files that you've changed.
- `git commit -m "<message>"` to "commit" these changes, and give a message about how you've updated things.
- `git push` to push your changes to the interwebs, and in a little bit, [https://bagels-bikes.github.io/](https://bagels-bikes.github.io/) should be updated!!!


Please ask me if you have any questions... if you can figure out how to reach me!!!

## How does it work?

I browsed reddit for some hours to see what web tech people like today. It seems like they are big fans of [eleventy](https://www.11ty.dev/) and [tailwindcss](https://tailwindcss.com/). The first one is for converting "template" files into good ol' HTML, and the second one gives you lots of easy built in styling stuff.

After working on this for a while, I think I still really like tailwindcss (I've fiddled with it before), but I'm not thrilled with my eleventy experience. Maybe I just don't know how to use it right, but I think next time I'll use something like react or vue and generate static HTML.

One last thing I should mention is that I use github actions to do the build process after you push, which you can see in `.github/workflows/deploy.yml`.

Hope this helps!