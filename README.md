# Automated inference: Reasoning in abstract argumentation frameworks

This system is an MIT licenced open source educational tool for visualising arguments and their attack relations and infering all the sets of arguments that can co-exist in a rational manner.

`Don't be quick to alter your understanding of argumentation theory if an inference is counter-intuitive. Although tested and evaluated, this appliciation may occasionally draw false inferences since debugging is an open ended task. Consult an expert if in doubt.`

## Demo
![Alt Text](https://media.giphy.com/media/2dbYilbYsuuskwfza1/giphy.gif)
## Prerequisites

All commands are directed at Mac and Linux users and should be parsed into a Terminal prompt.

  - Make sure you have Python 3 or above installed on your computer
  ```sh
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  brew install python3
  ```
  - Make sure pip3 is installed
  ```sh
sudo easy_install pip3
```
  - Install Graphviz via pip3
  ```sh
pip3 install graphviz
```
  - Install Pillow (formerly known as PIL) via pip3
```sh
pip3 install Pillow
```
  

## Run

The application runs from View.py

Make sure you're using Python 3 to run it.

 - Launch Terminal
 - Type "cd " (w/ space) and drag & drop the folder downloaded from github once unzipped.
 - Type
```sh
python3 View.py
```

## User Manual
### Adding Arguments and Attacks
To add an argument, click add.
Once the add window pops up, make sure your argument has a label.
Add attack relations in the "Attacks:" field by separating the different arguments attacked by a comma. All spaces are disregarded.

If you input an argument that doesn’t exist in the ”Attacks:” field, it will be added automatically.

You can optionally add the content of the argument in the description box.
If you want to add attack relations to a previously declared argument, you can always do so by pressing add, writing the label of the declared argument in the label field and adding the new attack in the Attacks field.

Note : Once an attack relation is established between two arguments, it can’t be revoked.

### Infering Semantics
Press evaluate on the bottom left to see the extensions computed.
You can always remind yourself of the arguments content by selecting your argument from the right hand side of the description box on the main window.

If some extensions are not of interest to you, press filter from the bottom right of the ”Semantics” frame and check the extensions you want to hide from the pop up window.
Once you’re happy press filter once more, from the pop up window to see it close and your semantics filtered.

If you want to see the skeptically accepted arguments under some semantics, select the extension from the bottom left of the semantics frame and watch it appear bordered in red in the argumentation framework.

You can add arguments at any time and update the semantics with the evaluate button once again.

`The system significantly slows down after the addition of 14 arguments so avoid going above that number.`

If, at any time you want to start over, press Clear from the bottom right hand side.

## Feedback

If you notice any bugs or have any efficiency improvements to propose, please push your code and I will review it.
If your contribution improves/fixes some part of the system I will merge your code and add you to the contributors.
If you're not a programmer, please report the issue or improvement proposal to pavlosmoros@yahoo.com .
