------------------------------------------------------------------------
This is the project README file. Here, you should describe your project.
Tell the reader (someone who does not know anything about this project)
all he/she needs to know. The comments should usually include at least:
------------------------------------------------------------------------

PROJECT TITLE:
PURPOSE OF PROJECT:
VERSION or DATE:
HOW TO START THIS PROJECT:
AUTHORS:
USER INSTRUCTIONS:
http://wdi.supelec.fr/boulanger/Projets/GreenFootEclipse-En
How to work on a Greenfoot project in Eclipse
1. Create a project in Greenfoot
2. Create an Eclipse project using the folder of the Greenfoot project.
3. Copy bluejcore.jar and greenfoot.jar (found in the Greenfoot bundle and in the extensions folder inside the Greenfoot bundle on MacOS) into the Eclipse project (you may put them in a `Greenfoot` subfolder).
4. Add these jars to the build path of the project.
5. Create a file named `standalone.properties` in your Eclipse project with the following contents:
    project.name=<The project name>
    main.class=<The name of the class of your world>
    scenario.lock=false
For example, you may have:
    project.name=Greenfoot in Eclipse
    main.class=MyWorld
    scenario.lock=false
6. Select your project and choose Run as > Java Application. In the list of possible main classes that pops up, select GreenfootScenarioMain` and click `OK`.
7. If your actors use pictures or sounds from Greenfoot, copy these ressources inside your Eclipse project. If these ressources are not at the top level of your project, edit the `project.greenfoot` file to fix the paths. For instance, if you put the pictures into an `images` folder in your Eclipse project, you will have to replace:
        class.MyActor.image=rock.png
with:
        class.MyActor.image=images/rock.png
8. Enjoy! 
