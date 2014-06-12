For each of the following elements, place them in what you think is the most appropriate pattern category (M, V or VM/C). To be clear, you should think of each of these elements not in terms of "who" requests the function, but "who" implements it (where "who" is a M, V, VM/C).

###Answers

- Create a new image with a star rating of 0
	- M
	- The star rating is data and associated with a business object (model).
	- This would need to perform validation on the image URL, name, etc before allowing it to be stored.

	
- Display the current star rating for an image
	- V
	- Displaying is always the responsibility of the View.

	
- Determine the total number of images that can have a 4 or 5 star rating
	- M (collection)
	- A maximum number of images with a 4 or 5 is a business rule that should be implemented in some form of Model containing a collection or count of ratings.
	- A Controller (VM) could also be used in this situation but the logic of how many images can have a 4 or 5 star rating should not be tied to a route or area of the page.

	
- Present a "add a new image" dialog
	- V (some directive)
	- All presentation is done via a view

	
- Change the star-rating of an image
	- All three
	- The view event will need to pass the new star rating to some form of business model representing the image so it can be saved, via the controller.  So V -> VM -> M.

	
- Show only starred images (1 or more stars)
	- V and Some service
	- A view is always responsible for 'showing', but this list of images should be organised by either the Model, controller or some other service that is not a part of MV*.  The view shouldn't be responsible for doing the complete filter however in Angular the view often is via a filter service.

	
- Show only images with NO stars
	- As above, V and either a collection, service or controller.
	- The presentation of the images is purely for the View but the logic of checking whether images have no stars is a higher level service such as a filter or collection/model method.

	
- Determine which star was clicked
	- V triggers event with some information about the click target, VM can receive this event and associate it with the star business object on the Model.
	- The view will own the click and pass it onto the model that will then be associated with the 'star' of the image.

	
- Who answers the question: "Can the current image have a 4 or 5 star rating?"
	- Service in collection(M) or VM
	- A service or collection could decide whether another image is allowed with 4 or 5 stars by counting existing image stars and making the decision based on configuration and business rules.  This should not be contained within the View as other parts of the application may need to access these business rules and respond to their change easily. 

	
- Reset an image's star-rating to 0
	- M, called by VM or data binding
	- The Model will be triggered by the view and routed through the VM, also this could happen externally without the use of a View.  The Model should eventually make this state update.

	
- Notify the user they can no longer add 4 or 5 star ratings to an image
	- Service/VM to V
	- Whoever made the decision about whether or not the user can add these star ratings would pass this information to the View for presenting to the user. 

	
- Maintains the set of selected images (for mass star-ratting)
	- VM or Collection of Models
	- Multiple models in a collection could have selected properties
	- Also another service to manage this information externally to the Model so that selecting the same image in different parts of the application don't necessarily effect each other.  This would then potentially tie the information to a local instance and be the responsibility of the Controller or some local collection.  It depends.

	
- Select one or more images
	- V -> VM -> M
	- The V could potentially trigger the select event but may not, it would then be routed to the C in the case of a local selection for a local copy of M or applied to the said image's M for a global application state change of the image.

	