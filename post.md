
##  What is this about 

As a self-taught  developer I know advice that is more  valuable on what to do is WHAT NOT TO DO. Anytime I work with a Senior Developer I finish my session asking 
 ```" What should I do to avoid doing to avoid this issue"
 -or -
 "How do I prevent this again?!" ```
 
  It is far too easy to google a tutorial or resolution to issue then find yourself in a far deeper hole that you can't just `rm -rf` your way out of.  


## Here are tools that can help you avoid hours of debugging in the future
###Set your Path! 
  No this isn't personal life advice.  The path I speak of is the $Path on your computer. Not setting a path correctly  can cause you to save packages/gems  (even when you try you save globally ` -g `)  in hidden places rendering them useless.  This may seem like a no-brainer to some of you but I have pulled hairs out wondering why `Rails new` or `NPM install` would not work after installing 4 times! Also having multiple installation of Node or Rails on your local enviroment  is an embarrasing mistake.  
  
 Here are some simple instruction to set Path variables ( on a Mac)
  <ol> 
  <li> Open up a Terminal window (this is in your Applications/Utilites folder by default) </li>
  <li> Create a back profile and open in editor .
        `touch ~/.bash_profile; open ~/.bash_profile` 
  </li>
  <li> Add the following line to the end of the file adding whatever additional directory you want in your path 
    `export PATH="$HOME/.rbenv/bin:$PATH"` 
 </li> Save the .bash_profile file and Quit the editor </li>
 <li> Deploy the new bash profile 
 `source ~/.bash_profile`
 </li>
 <li> Done! Now you can check you path `echo $PATH` </li>

###  Use Package Version Management 
 This can help with future dependency issues.  No one needs to re-invent the wheel so its highly likely you will use some Ruby gem or Javascript module for  to save time .  Well over eventually one gem or JS modules will fall behind on updating to newest Node or ruby version. So please use 
 
 <ul>
 <li> [Node Version Manager aka NVM](https://www.npmjs.com/package/nvm)</li>
 <li> [Ruby Version Manager aka RVM](https://rvm.io/)</li>
 </ul> 
 
 Installation is fairly simple but now you can specifiy which version of node or ruby enviroments to use.  This can be especially helpful when using a variety of ruby gems that are yet to be tested on the newest ruby package. 
 
 ### What else
   I will be posting more advice as I continue to make mistakes on my journey to Senoir Dev .  
 


