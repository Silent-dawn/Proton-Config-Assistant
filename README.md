# Proton-Config-Assistant

![logo](../main/readme-assets/Nightowl_ascii.png)

A script designed to help people configure their Proton arguements for Steam.

With the many flags and arguements available, it can be cumbersome to remember them all.

This is a tool designed to address it in some manner.


---
## TODO
---

- [x] Add Wine DLL Override support & FSR support
- [ ] Add Intel GPU support
- [ ] Break up codebase into non-monolithic functions
- [ ] Create a reference/index of flags
- [ ] Clean up input capture method

---
## Features
---

- Support for AMD and Nvidia specific options, including Nvidia NGX.
- Support for adding in custom Wine DLL overrides
- FSR support
- Support for disabling forms of DirectX
- Suppport for forcing Wine OpenGL
- Nvidia Shader Cache support
- And More!

---
## FAQ
---

Q: I can't run the file!\
A: run `chmod +x` on the file  

Q: I hate the logo, can I get rid of it?\
A: Sure can, remove any references to the `Introduction` function, or replace the logic with something you prefer.  

Q: Why is there no IF in your code?\
A: I use case statements and test operators to bypass the need for if. Long story short, its for performance.  

Q: What does stuff like `Grey="\e[38;5;248m"` do?\
A: They are ANSI escape codes so I can make colors easier to impliment in code.  

> [!NOTE]
> Check this gist out to learn more: [Link](https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797)

Q: What is going on in code like this?\
    `while [[ $(grep -E -q "^[yYnNeEoOsS]{1,}" <<< "${PromptOutput}")${?} != 0 ]]; do`\
A: It's a while loop that uses test (the `[[ ]]` part), grep, heredocs (the `<<<` part), and last process exit code (`${?}`) to check for valid input.  

Q: Why does your code not follow (insert name here) convention?\
A: I'm a self taught goofball on the internet, and this isn't a professional product.  

Q: How do I make a feature request?\
A: Create an issue on Github and I'll check it out.  
