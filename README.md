# Peristéri (Perist-ri)

## Peristéri 2.0 has been released! No need for python at all. All you need is your shell
Check out https://github.com/Stylo2k/Perist-ri/tree/2.0



### [Latest Features](#new)
- Installable as a binary file
- Multiple Files Submissoin
- Now In, Out, Expected, Error & Diff files


Submit to Themis through command line and get Themis's feedback.

Successful submission attempt:
    ![][overview]

Failed submission attempt:
    ![][failed]
Here you get to see the reason and the hint

Multiple Files Submission:
    ![][multiple_files]

In, Out, Expected, Error and output files:
    ![][show_files]

Browser Mode:
    ![][browser]

---

## Table Of Contents:
1. [ Requirements ](#desc)
2. [ Installation ](#install)
3. [ Usage ](#usage)
    1. [Through command line arguments](#cmd)
    2. [As a command line browser](#browser)
4. [New features](#new)
4. [Coming features](#coming)

---


<a name="req"></a>
## Requirements
1. Git
    > [windows](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git/#:~:text=Installing%20on%20Windows)

    > [mac](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git#:~:text=com/download/linux.-,Installing%20on%20macOS,-There%20are%20several)

    > [Linux](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git#:~:text=work%20just%20fine.-,Installing%20on%20Linux,-If%20you%20want)

2. Python3
    > installation guide [here](https://realpython.com/installing-python/)

3. Pip (python3-pip)
    > look it up for your OS (operating system)
<a name="install"></a>
## Installation

    > git clone https://github.com/Stylo2k/Perist-ri.git
    > sh install.sh

## First time configuration
For the first time configuration you will need to specify your student number (with a lower case s) and your password
This data will get stored locally in :

    ~/.themis_submitter/data.yaml

<a name="usage"></a>
## Usage
<a name="cmd"></a>
### Through command line arguments
    > submit <files to submit> <submission url>

Or to see the in, out, expected, error and diff flies:

    > submit <files to submit> -y <submission url>

This will simply submit your file to the url you specify. This is the cleanest way to submit. But since not all people will prefer this way. You can use the browser method.

Having trouble with the submit ? Try :

    > python3 ~/.themisSubmitter/Peristéri.py

Or just 

    > ~/.themisSubmitter/Peristéri.py

<a name="browser"></a>
### As a command line browser
    > submit
This will let you browse Themis just like you would in your browser. BUT of course through the terminal.

You can specify to what directory you want to go with numbers (indices). When you are at a submittable page, you will get asked if you want to submit or go back. When you submit a small window will open to get you to choose the file you want to submit.
<a name="after"></a>
### After submission

After submission your submitted file wil get judged and the test cases you passed/failed will get prompted in your terminal. If you pass all test cases the program will terminate. Otherwise, you are given the chance to resubmit.

<a name="new"></a>
# New feature !
The usage is now different and way better than the previous one. Instead of having to locate the `.py` file when submitting each time, you actually install it on your system as a `bin`. So you can use it now as any command you are used to in the terminal.
See [submit.sh](submit.sh) (30-nov-21)

    > submit
This feature does not work on all distros tho. If you are having trouble with this feature, use
    
    > python3 ~/.themisSubmitter/Peristéri.py

You can now submit multiple files !!!! (04-12-21)

    > submit <file 1> <file 2> <file...> <link>

You can now see the in, out, expected, error and diff files !

    > submit <file1> <files...> -y <link>

<a name="coming"></a>
# Coming features

1. [x] Make the program installable as a `bin`
2. [x] Multiple Files submission
3. [x] See in, out & difference test files
    - [ ] Add this to the browser mode
4. [ ] Encrypting the data
5. [ ] Better name for `.Py` file
6. [ ] More documented code
7. ?

[overview]: resources/Screenshot.png "alt"
[failed]: resources/failed.png
[browser]: resources/browser_mode.png
[multiple_files]: resources/mFiles.png
[show_files]: resources/show_files.png
