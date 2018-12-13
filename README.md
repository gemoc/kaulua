Kaulua
======

Kaulua is a research collaboration between [Obeo](https://www.obeo.fr/en/) and the [DiverSE team](http://diverse.irisa.fr/).
This collaboration is studying distributed modeling environment through the PhD of Fabien Coulon.


Motivation
----------

There is currently a trend towards the implementation of Integrated Developpement Environments (IDE) with web technologies.
This happens for two main reasons. 
First of all, web technologies are now mature and outperform traditionnal desktop technologies in terms of user interactions, especially when it comes to developping graphical interfaces.
Seconds, users are increasingly demanding online services such as data storage, computing power, ready-to-use applications and want to collaborate in real time with others.

To give some examples of developpement tools following this trend, there are VS Code (an IDE implemented only with web technolgies), Eclipse Theia (an IDE usable in Web or desktop setting), Eclipse Che (a web IDE coupled with a workspace server), Eclipse Orion (a web IDE), Sourcegraph (an online and smart code reviewer on top of Git repositories), Atom (code editor implemented with web technologies), etc... <br>
In addition to these tools, the IDE community is working to agree on a common protocol, the Language Server Protocol (LSP) to communicate with a Language Server from an IDE, the idea being to to separate IDEs from their language services (diagnostics, goto, diagnotics) to make them reusable in any IDE.

Next to IDEs, modeling workbenches (Domain-Specific IDE specialized in model manipulation) are still desktop applications. But since their users have the same needs, the modeling workbench will have to migrate to web technologies. 

Modeling workbenches are similar to IDEs but have also specific concerns.
Models are mainly manipulated through non-textual representations (diagram, tree, form etc...) but LSP focuses on textual languages and the supported language services do not fully meet needs of a modeling workbenches. For example, services such as 'goto implementation of a method' may be useless for a diagram editor and services such as 'computing a layout for a diagram' are missing.

We have three motivating scenarios for this PhD:
 - Distributed modeling environment :
   The languages services are deployed at several sites, including remote manipulation services for the workspace and a browser interface for the user interactions with the modeling workbench.
 - Collaborative modeling environment :
   Multiple users share and edit models simultaneously.
 - Reconfigurable modeling environment :
   The deployment of language services is dynamically reconfigured to adapt to changing user needs.

Objective
---------

Since the current Web IDEs have a Client-Server architecture that doesn't allow a finely granulated deployement of the different languages services, the objective of the PhD will be to study micro-service architecture for modeling environment in order to support the motivating scenarios.


We will focus on tree main axes of exploration:
 - A communication protocol between the various language services
 - Automatic deployment of the different language services
 - A mechanism for dynamic reconfiguration of the deployment


Publications
------------

**Shape-Diverse DSLs: Languages without Borders** (SLE’18 best vision paper) <br>
Fabien Coulon, Thomas Degueule, Tijs van der Storm, Benoit Combemale <br>
In *Proceedings of the 11th International Conference on Software Language Engineering* (SLE), 2018.
[doi](https://dx.doi.org/10.1145/3276604.3276623) [preprint](https://hal.archives-ouvertes.fr/hal-01889155)

Involved people
---------------

Fabien Coulon - Obeo / Université Rennes 1 / Inria

Stéphane Bégaudeau - Obeo

Mélanie Bats - Obeo

Benoit Combemale - Université Toulouse Jean Jaurès

Olivier Barais - Université Rennes 1

