# Engineering Guidelines
**So here you are. When in doubt, as they say, read the (ahem) manual. :)**
Below is a list of guidelines for working productively on the engineering team at Shopl. We strive to write easy, clean, code as much as possible.


## Philosophy
*No matter what language you are writing in, here at Shopl we strive for code that mirrors "The Zen of Python", a  collection of 19 "guiding principles" for writing computer programs that influenced the design of the Python programming language.*

**The Zen of Python**
By: Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!

## Coding Standards

All code in any code-base should look like a single person typed it, no matter how many people have contributed. 

Code refactoring should **NOT** be done just because we can. Yes, the coding standards are important, but refactoring older files simply to conform to the standards is **not** an urgent issue.

All new or updated javascript based code will be reviewed to ensure it conforms to the standards and passes the linter.

### Spacing in JS

***We are a proud tabs family.***

 - Indentation only with tabs
 - No whitespace at the end of a line or on blank lines
 - Lines should be no longer than 80 chars (counting tabs as 4 chars)
 - If/else/for/while/try blocks should always use braces and go on multiple lines
 - Any `,` or `;` must NOT have preceeding space
 - Any `;` used as a statement terminator MUST be at the end of a line
 - Any : after a property name in an object definition must NOT have preceding space
 - The ? and : ternary conditional MUST have space on both sides
 - NO filler spaces in empty constructs
 - There should be a new line at the end of each file
 - All function bodies are indented by one tab even if the entire file is wrapped in a closure
 - **ONLY TABS SHOULD BE USED AT THE START OF A LINE OR TO ALIGN CODE WITHN DOCUMENTATION BLOCKS OR WITHIN A LINE**

Whitespace can easily accumulate at the end of a line - avoid this. One way to catch whitespace buildup is enabling visible whitespace characters within your text editor.

### Documentation
Each repository we make should have a detailed and up to date README file in its root. This is so that every team member can have a clear and concise overview of how to engage with the repository at any given time.

You can delete the current file by clicking the **Remove** button in the file explorer. The file will be moved into the **Trash** folder and automatically deleted after 7 days of inactivity.

## Development Lifecycle

 1. **Creating Branches**
	Branches should be created off of the master branch and must be named ONLY "your-name"
 2. **Writing Code**
		Please refer to coding standards
 3. **Writing Commits**
		Commits should begin with your taskID and describe what you did. Keep it Short & Simple!
 4.  **Creating a Pull Request**
- All pull requests should point to the development branch
- The pull request should ALWAYS include the taskID
- The more detailed the pull request the better: 		
-- A screenshot of the UI, if PR implements or fixes it 		
--A gif image if any animation is part of it 		
-- Text description of what reviewers should pay attention to during code reviews
- When merging down to your local machine always pull from DEV
-- Merge conflicts should always favor the dev branch
-- Always be sure to stash your local branch if merge conflicts occur
5. **Code Reviews**
	Make two passes over the PR if its substantial 

# Readme Guidelines
Each repository should include a README in the root of the directory. The README should be detailed enough that any engineer just starting should have a clear overview of the project and be up to data. 


## Project title 
A detailed overview that explains **what** the project is about.


## Build status
Build status of continuous integration i.e. travis, appveyor etc. Ex. - 

[![Build Status](https://travis-ci.org/akashnimare/foco.svg?branch=master)](https://travis-ci.org/akashnimare/foco)
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/github/akashnimare/foco?branch=master&svg=true)](https://ci.appveyor.com/project/akashnimare/foco/branch/master)

 
## Screenshots
Include logo/demo screenshot etc.

## Tech/framework used
*(Be sure to include if this project needs any dependencies from other projects and link to them as well)*
Ex. -

<b>Built with</b>
- [Electron](https://electron.atom.io)

## Features
What makes your project stand out?

## Code Example
Show what the library does as concisely as possible.

## Installation
Provide step by step series of examples and explanations about how to get a development env running.

## API Reference

Depending on the size of the project, if it is small and simple enough the reference docs can be added to the README. For medium size to larger projects it is important to at least provide a link to where the API reference docs live.

## Tests
Describe and show how to run the tests with code examples.

## How to use?
Describe how to use the project/library and provide examples.



