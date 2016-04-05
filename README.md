## Introduction
This short exercise will help you understand the power of Web Components using Polymer 1.0

## Step 0
Let's start by installing [node.js](https://nodejs.org/en/download/), [bower](https://github.com/bower/bower) and [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) on our computers.  
Clone or download the contents of the repository from [GitHub](https://github.com/CalinGinga/polymer1.0). 
* Download [ZIP](https://github.com/CalinGinga/polymer1.0/archive/master.zip) or
* git clone git@github.com:CalinGinga/polymer1.0.git

Let's discuss about the contents of the folder

Start the web-server by running "node ./scripts/web-server.js" from the root directory

## Step 1
Inside the index.html file create a simple HTML list with each list item containing a span with the name of an ice cream and a paragraph with the description:
* name = Napoca Panda / description =  Inghetata cu cacao si inghetata cu aroma de vanilie
* name = Napoca Lux / description = Inghetata cu cacao si cu aroma de vanilie, cu glazura cu cacao si alune

After the list create a paragraph with the a hardcoded total number of ice creams.

## Step 2 
Create an elements folder and inside the folder create your first web component file called *ice-cream-list-item.html*. Inside the file create a template for an iceCream element. You will need a *div* containing a *header* element for the name and a *paragraph* element for the description.  
After the template create a script containing the definition of the Polymer web component.  
Add some styling to the template.  
In the *index.html* file replace the HTML list with two ice cream items.

## Step 3
In the elements folder create a new html file named *ice-cream-list.html* containing a template for the list.  
In the script section define the list and create the _iceCreams_ object which will have popularity, name and description. Also we will add more ice creams:
* name = Napoca White / description = Inghetata cu lapte si glazura alba cu alune
* name = Magnum Almond / description = Inghetata de vanilie cu ciocolata cu lapte si migdale
* name = Magnum Infinity Chocolate / description = Inghetata cu ciocolata si sos de cacao, cu sos de ciocolata neagra si bucatele de boabe de cacao.

Replace the ice cream items from the index.html file with the new ice cream list.

## Step 4
Add a sidebar search to the left of the table of ice creams. Create a *div* containing a *search* input, a *current search* section and a *number of results section*.  
In the script section add properties on the prototype for the filter. You will need to create a property for the filterText with type, observer and the default value, define the iceCreams as Array and currentIceCreams property with type and the computation method.  
The methods that need to be created are the observer mentioned above (*filterTextChanged*), the filter (*iceCreamFilter*) and the method for getting the current ice creams (*getCurrentIceCreams*).

## Step 5 
Replace the *current search* section with a sorter based on a criteria. Set the sorter as being a checkbox for descending and ascending order. Add two properties one being the *criterium* and one being the *descendingSort* property. Make modifications to the existing methods so that the sorter applies and create an *iceCreamSorter* function that inverts the order.

### Congratulations on finishing the 5 steps to a catalog application with search and sort functionality using _Polymer 1.0_!!

