# My Vue Learning Experience

These are my notes to myself and to anyone else who might learn a few things by reading my experience
on windows trying to get some vue stuff going.

## Installing and getting setup to actually code.

I already had VScode installed, so I hunted for some form of runtime related to the extensions.
No dice, so I went to [the node website] and ran the installer to install 14.17.5 directly after wasting
20 minutes looking around for a way to run nvm on windows. 

Once I got that going and had _restarted_ vscode, I could now run commands from my git bash terminal
I had configured in vscode before hand. So,

    npm install -g @vue/cli

Then, following [a tutorial on the vs studio website], I ran the create command:

    vue create blackjack

That made a folder for me. So I guess that's how we'll roll this. Multiple subfoders in here. That's fine,
we're learning and I'll probably make some new projects at some point. Anyway, moving along, I want to have
bootstrap around so that I can use it for whatever I'd like and so I don't have to think about styles. So I
looked up the boostrap vue page and ran another npm command.

    npm install vue bootstrap bootstrap-vue

Then I followed the instructions on the [bootstrap docs page] to add some use commands that probably do... something.
After doing that, I played around with the html a little. Removing the default component text and adding in some bootstrap
components to make my dopamine levels jump up. But, then I made a mistake and deleted some files sitting at the root level
directory of git repository. Which somehow broke everything in the blackjack folder... what?

So, I ran the vue install cli and create blackjack. Luckily git exists. So, I didn't actually lose anything when it overwrote
everything despite my selection of the 'merge' option. Figure that out. Anyway, I ran the bootstrap install commands again
and watched as it created a package-lock.json file at the root again. So. Weird. Putting that aside, next install command!

    npm install vuex

Because I want a store and I want to learn how!

[a tutorial on the vs studio website]:https://code.visualstudio.com/docs/nodejs/vuejs-tutorial
[the node website]:https://nodejs.org/en/download/
[bootstrap docs page]:https://bootstrap-vue.org/docs