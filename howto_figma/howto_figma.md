# HowTo Figma [^1]

Target group: readers interested in (collaborative) UI (unser interface, website) design, with or without prior knowledge in UI design

Contents: introducing Figma as a tool for UI design, exemplified by designing - step by step - a simple UI for a (fictional) digital-edition project

Aims: readers can use Figma to (collaboratively) plan and design UIs

## Introduction

Figma is a tool for collaborative UI design. It can be used for interface mock-up (realistic visual design) and prototyping (realistic visual design plus simulation of interface functionalitites). Mock-up and prototyping will usually not be the first steps in interface design: they will usually be preceded by other steps such as expert interviews, brainstorming, or use case modeling. Most especially, mock-up and prototyping are typically preceded by [wireframing](https://en.wikipedia.org/wiki/Website_wireframe).

## First Steps

### Sign up

Figma can be used through a [web-based application](https://www.figma.com/). There are different pricing options including a free `Starter` plan with limited numbers of files as well as `Professional` (free for students and educators) and `Organization` plans (March 2022).

### Create a Team

Create a team to collaborate. Right at the start, Figma will ask you to name your team and to invite your collaborators. For trying Figma, choose the `Starter` team plan. (You can work in Figma individually as well. If you want to skip creating a team for now, you can later select `+ Create new team` in the bottom-left part of the start screen). In the example project, the team's name is `Awesome Poetry` and consists of two members.

![image of the Figma start screen](howto_figma_1.png)

## Mock-up

### Create a Design File

Create a design file by clicking `New design file`, or by clicking the `+` icon that will appear next to `Team project` when you hover over it and selecting `Design file`. This will open the workspace screen.

![image of the Figma workspace screen](howto_figma_2.png)

The first step is to create a frame that represents the start page of your future website. When you click on the `Frame` icon (the third icon from left in the top navigation bar of the workspace screen, part of the `Region tools` dropdown menu), the bar on the right-hand side will offer predefined sizes of frames that correspond to different devices for accessing your website. For our digital edition of awesome poetry, select `Desktop` size (1440 x 1024 px). In the left-hand `Layers` area, double-click the name of the frame ("Desktop - 1") to rename it "StartPage". **It is always good to give telling names to your objects in order not to get confused - there will soon be a lot of them.**

### Create sub frames

We can now start adding sub-frames within the "StartPage" top-frame to define large areas within the page. Let's first create a navigation bar: select `Frame` and draw an oblong shape in the top part of the page. In the `Layers` area, rename it "NavBar". The width and height are displayed in the right-hand `Design` area of the workspace screen (and next to the frame whenever selected). Further below, in the `Fill` segment of the `Design` area, you can pick a color. In the example, a dark blue has been chosen. As this color will be used as one of the edition UI's signature colors, it can be saved: next to `Fill`, click on the four-dot icon which the tooltip identifies as the `Styles` button. Then, select `+` and name the color style, say, "EditionBlue". Now, you can easily come back to that color when you need it.

![image of the "StartPage" and "NavBar" frames](howto_figma_3.png)

Add three more frames. A large frame below our "NavBar" as the "MainFrame"; a smaller "FunderFrame"; and an even smaller "ImprintFrame". Give the "MainFrame" an off-white color and save the color as "EditionWhite". Give the "FunderFrame" a thin border: in the `Stroke` area of the right-hand dialogue bar, click the four-dot icon and select the "EditionBlue" hue to apply the saved color style; set the line width to "1". Leave the "FunderFrame" white and make the "ImprintFrame" grey. In the right-hand `Layers` navigation, arrange the frames according to their position on the page.

### Populate w/ Objects

You can now start adding objects to the frames. In the `Shape tools` drop-down list (the fourth icon from left in the top navigation bar of the workspace view), pick `Ellipse` and, in the blue navigation bar of your own page draw a circle. Color it in "EditionWhite" and rename it "APLogoShape". Furthermore, add some text onto it (such as "AP") by selecting the `Text` icon (sixth icon from right in top navigation bar of the workspace). You can style that text (font, size, style) via the `Text` section of the right-hand tool space; you can select the "EditionBlue" hue by clicking the four-dot icon next to `Fill`. Rename the text object "APLogoText". Also, add a `Rectangle` as well as a text to represent a drop-down button. Style and rename as "DropDownShape" and "DropDownText", respectively.

Add three text objects to your "MainFrame": a title, a subtitle, and some introductory text. Also, add a rectangle and a text to represent a search field. In the "FunderFrame", add a shape and text to represent a funder's logo. Moreover, add a text, representing a link, to your "ImprintFrame". Style those objects and rename them as useful. You can arrange their order in the left-hand `Layers` bar--for example, when a text object gets hidden behind a shape object and is no longer visible.

### Group Objects Together

It is useful to group together objects that belong together, for example, objects that together constitute a more complex object. In the `Layers` bar, select both "APLogoText" and "APLogoShape", right-click them, and select `Group selection`. Rename the created group "APLogo". Likewise, create "DropDown", "StartPageText", "SearchFunction", and "Logo" groups. Select those group names in the `Layers` area in order to target the complex objects (instead of their parts). (At this point, you might wish to collapse the layers in the `Layers` area below the group level.)

### Create Components

If there are objects, or complex objects (groups), that are used more than once in unaltered form, you can create components that can be easily reused. In the `Layers` area, right-click the "Logo" group and select `Create component`. (You can also click the `Create component` icon in the middle of the top bar of the workspace.) As a component, it is now highlighted in purple color.

Change the view from `Layers` to `Assets`. In that area, you will find the "Logo" component below "StartPage". From here, you can drag-and-drop that component multiple times onto the "FunderFrame" to represent the logos of several funders. Please note, that if you change the original component (designated by a four-diamond icon in the `Layers` area), all its instances (rombic-shape icon) will be changed in like fashion. On the other hand, if a component's instance is changed, the other instances as well as the original component will remain unaltered.

At this point, you might wish to see your page in presentation mode (rather than work mode). For this, click the `Present` arrow (second button from right in the workspace navigation bar). The work mode will remain active in another tab.

## Prototyping Interactive Functionality

### Add another Page

By means of adding even more objects, groups, and components (to represent, for instance, images), you can thus create visually compelling mockups of your page design. However, Figma lets you also prototype functionality by simulating user interactivity and navigating between pages (or within different areas of the same page).

Suppose that the "Imprint" text on the bottom of your "StartPage" is meant to represent a link to another page that contains legal information about the website's publisher. So, let's build another page. Create a second desktop frame as you did above--it might be useful now to zoom out of the central window of the Figma workspace so that you can see both pages. Rename the new page from "Desktop - 1" into "ImprintPage". Whereas we will leave that new page blank, you would usually want to design it in a way that is similar to your "StartPage". (Among other things, you might want to create a "NavBar" component and add it to the top of all your pages.)

### Create Variants of a Component

Turn the "ImprintText" object into a component (as we have done it above). Subsequently, drag-and-drop it from the "StartPage" frame into the grey area that surrounds it. In the `Layers` bar, it will no longer be shown within the "StartPage" hierarchy, but on the same level as both the "StartPage" and the "ImprintPage".

Now, what we want to do is create two different variants of our "ImprintText" component that correspond to two different types of user interaction:
1. "Default": there is no user interaction,
2. "Hover": a user's cursor hovers above the "ImprintText".

Keep the "ImprintText" component selected. In the right-hand control area, click `Variants`. Our component has now automatically been duplicated. The lower twin of the component should be highlighted; in the right-hand `Variants` area, enter "Hover" to designate `Property 1` (instead of "Variant2"). (When you highlight the upper variant of our component, its name should be "Default". Leave it like that.)

Now, we can design what it should look like when a cursor hovers about the "ImprintText". Twice double-click into the text and style it bold. 

The next step is to define the interaction that triggers the "Hover" variant. To that end, select the (upper) "Default" variant. In the top of the right-hand control area, switch from the `Design` tab to the `Prototype` tab. Next to `Interactions`, click on the `+`. In the `Interaction details` window that pops up, choose `While hovering` - `Change to` - `Hover`. Close the window. As long as the `Prototype` tab is active, the "Default" variant is now connected to the "Hover" variant through a purple arrow, indicating that the former will change to the latter when an event (a hover event, in our case) takes place.

However, we also want the "ImprintText" link to the "ImprintPage". For this, highlight the lower, "Hover" variant of the "ImprintText" component. In the `Prototype` section, click `+`; and select `On click` - `Navigate to` - `ImprintPage`. A blue arrow now depicts the linking to the "ImprintPage".

The "ImprintText" component is now fully configured and an instance of it can be implemented in the design of our "StartPage". From the `Assets` bar, beneath `Local components`, drag-and-drop the component (showing the text "Imprint") to the "ImprintFrame" of our "StartPage". Switch to `Present` mode and try out the hover event and linking.

### A More Complex Example: Create a Dropdown Menu

There is an empty "Drop-down" button in our "NavBar"


...

select lower variant
click +
copy all objects from ...
hightlight variant 3 object
paste

rename Variant3 into Click
Variant4: Hover1
Variant5: Hover2

On Click change to Default
While hovering change to Hover1
While hovering change to Hover2

fairly complex network of interrelations

drag-and-drop from Assets to NavBar frame of StartPage
however, in Layers move from NavBar frame to StartPage frame (otherwise appearance restricted to the NavBar frame space)

click play

easy to see how dropdown instances can be customized:
change texts, create interactions to link to other pages (still to be created) upon click events

add link to sample page

alternative ways to reach same objectives;
many more objectives;
large number of tutorials




 In the `Layers` area, select, first, "DropDownText" (in the layer beneath the "Hover" component variant) and, second, "DropDownShape", and inverse the colors ("EditionBlue" for the text, "EditionWhite" for the shape). Leave the "Default" variant as it is.

However, we need another variant to simulate what happens when a user actually clicks on the button. Highlight the "Hover" variant in the central screen and click on the `+`. In the right-hand `Variants` area, rename "Variant3" into "Click". 


eg: hover state and default state as two variants of a button component

'variants + in' right-hand side bar

eg property is "state"

name variants eg state=default and state=hover

add interaction

tab prototype

select one state, select interaction +

choose interaction for first state, such as 'while hovering' 'change to' second state

add component (again) where you need it and the interaction will be added

(there are many public plugins that can be tapped for standard functionalities such as drop-down menus etc.)

constraints can be used for responsiveness

you can export css code from figma (developer handshake)

in order to link from fields/buttons to other pages: select interaction 'on click' 'naviage to' another top-level frame

'scroll to' other frames on same page (animated or not)






[^1] Based on contents provided by Fabian Etling (CeDiS, Freie Universität Berlin) at ide 2022 Winter School Digitale Editionen - Interface-Design, University of Wuppertal, 21-25 Mar 2022.