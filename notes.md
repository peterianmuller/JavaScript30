data attributes is if you want to make up an attribute for an html element. In this case we'd like to link up our <kbd> tag with an audio tag. We give both the same data-key attribute.

<div data-key="65" class="key">
  <kbd>A</kbd>
  <span class="sound">clap</span>
</div>

<audio data-key="65" src="sounds/clap.wav"></audio>

adding event listeners. We add an eventListener to some html element as a property and then add the specific event we're listening for, the nthe funciton that we want to run.

window.addEventListener('eventName', ()=>{})

es6 backticks. This says eerything is a string literal until we see $ with curly braces, which is JavaScript.
const audio = document.querySelector(`audio[data-key="${e.keycode}"]`)

transition property on css

Problem with setting setTimeout in JS to end class assignment. With a transition rule in our css we would have to sync up our JS to CSS and if any time stuff changes from css to JS things could get out of sync.

transition end event

when we add an event listener we must add event listener to each element, not just the array we get when we run things like querySelectorAll('.key'). Running this method will give us a node list and we have to access each node list and add events.

nodelist vs array -> nodelist methods much more limited than array methods. document.querySelector will give back a nodelist

this.dataset is a property on the node that will select all of the data attributes from a certain element. We gave data-suffix values to out two inputs that require px and none to our input that chooses color.

We have these CSS variables described in the :root and we have given a name atribute to the input elements. This is how we are going to update those variables.

When you use CSS variables, you can use JS to update thier values so that they update wherever they are scoped on the page. This is an interesting example of scoping in CSS
