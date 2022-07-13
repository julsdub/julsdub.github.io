13/07/2022

Good Morning, good afternoon or good night, but for me is mornig. I recived a call one hour ago from the organizer of the cybersecurity course, finally we start tomorrow, 15 days later than the originall date from start.

I started the day watering the plants that I have in the terrace, this terrace save my life during pandemics. After that I prapared a good cup of coffe and here I am writing some lines. 
Today I'll explain you how to setup a blog on github pages. it's what i'm doing know while I wait during ruby installation

The requirements for starting your own blog with github pages

You will need a Github account If you don't have it already. https://github.com
It's easy, you only neeed to write your email address into the box and click sign up for github.
After that you need to create a repository in your github. I will not go in deep in this topics because there are a lot of webs and tutorial explaining the same, and official docs

https://docs.github.com/en/get-started/quickstart/create-a-repo

when you finish creating your account and repo you may need to install homebrew, ruby and jekyll

What the hack is Hombrew? Is a packet manager, https://brew.sh explains better than me.

You need to copy and paste the line below into your macos terminal.

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

You don't know where is your terminal in mac? I'll show you

You have different options, 
- my favourite is Command + Space ( + space), this opens spotlight, a powerful search engine, write  Teminal and click.
- Another way is going to your dock, click on launchpad go to others an there you will find terminal.
- The last one is open finder, on the left go to applications, then find inside the folder call utilities and find terminal app inside
- If you dont have fovourites enabled go to your Hardrive in my case Macintosh HD/Apps

Macintosh HD/applications/utilities

When we finished the install we need ruby, and we are going to use brew for that

copy and paste in terminal:

brew install chruby ruby-install

install last stble version of Ruby

ruby-install ruby

after that we need to tell our bash to work with chruby, copy and paste in terminal

echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc

echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc

echo "chruby ruby-3.1.1" >> ~/.zshrc

this is runninng zhs shell if you run bash you may need to replace .zshrc with .bash_profile

Here you will find nice site and how to find out wich shell are you using.

when ruby is installed  close and reopen terminal and check for version

ruby -v

Now you need to install jekyll

gem install jekyll

install jekyll bundler

gem install jekyll bundler

Now it's time to create your site, navigate to your cloned reository and run 

jekyll new

after modifying some aspects in GemFile

its time to bundle and exec and serve jekyll

bundle exec jekyll serve --drafts --livereload

