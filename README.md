#Instructions to add simulations to the website

1. Go to `.app.js`
	write:
	`const name_of_Router = require('./routes/<name that will show in the URL>');`

	write:
	`app.use('/simulations/<name that will show in the URL>', name_of_the_router);`

2. go to `.route/simulations.js`
	add an element to the array on top of the file following the same structure as the ones you find there
	create a js file with the name of the simulation you are adding. Inside this file write down the same stuff you will find in single_pendulum.js but adapted to the simulation you are adding

3. go to `.public/javascripts` and add your simulation!


The idea is that `app.js` takes from `.route.simulations.js`, which takes from `.public/javascripts`

4. test to check if the simulation is in place
	if there are misaligned elements:
		do this for the canvas and any misaligned elements
		`<element>.parent('simwrapper');`
