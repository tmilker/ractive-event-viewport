ractive-event-viewport
======================

Event to fire when an Element has come visible from invisible state or vice versa.


Example usage :
    
     <script src="lib/ractive.js"></script>
     <script src="lib/in-view.js"></script>
	   
	   
Then use it like below  
      
     <div on-viewport="someFunc"></div>
     
     ractiveObj.on('someFunc', function(event){
        event.original.current // Current state
        event.original.previous // Previous state
        event.original.visible // visibility state, you can use event.original.current
     });

Please checkout http://svapreddy.github.io/ractive-event-viewport for more details.

<b>Limitations</b>

It does not work, if the target element's any of the parents have 0px height. Will fix it.
