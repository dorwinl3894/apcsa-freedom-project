# Entry 3
##### 1/5/20

### Update
My partner, Alex, and I have been tinkering with a lot of stuff in the past four weeks including three.js, typescript, java, javascript, c++, tinkercad, and blender. We have finally decided on something to make and it involves using Three.js , which is a javascript framework for creating web based games, Typescript for back end servers, and blender for 3D models. 

### Sources I am using for this project. 
For this project, I will be focusing all of my attention on learning Blender and Three.js. I have found many useful sources to learn both Blender and Three.js. Most of my sources are from Youtube because there are just a lot of it and you can ask questions on the comment if you have a question that the creator of the tutorial might be able to answer. 
For Blender, I am currently learning through these sources.   
[Blender Beginner Tutorial Playlist by Blender](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)   
[MODELLING For Absolute Beginners - Blender Tutorial](https://www.youtube.com/watch?v=ICBP-7x7Chc)   
[Blender 2.8 Beginner 3D Modeling Tutorial](https://www.youtube.com/watch?v=elUJCEC06r8)   

For Three.js, I am currently learning through these sources.    
[Three.js Tutorial for Beginners Playlist](https://www.youtube.com/watch?v=uzkedMF-l4Q&list=PLbu98QxRH81KkLTN00OXhD8Y-pRVgTCnM)   
[Three.js 10 part series](https://www.youtube.com/watch?v=YKzyhcyAijo)   
[Three.js Demos](https://threejs.org/examples/#webgl_effects_peppersghost)    

### Engineering design Process
Currently, my partner and I are at step five of the EDP, which is planning the most promising solution. I am currently educating myself on Blender and Three.js so that I am able to make a extremely simplified version of the game that I am trying to make. Using resources from the [official three.js website](threejs.org), I was able to make something appear on the screen using the three.js soure.    
The code that I had obtained from the website is 
```javascript
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>My first three.js app</title>
		<style>
			body { margin: 0; }
			canvas { width: 100%; height: 100% }
		</style>
	</head>
	<body>
	    <script src="https://threejs.org/build/three.js"></script>
	    <script>
	    //Creates a scene
	    var scene = new THREE.Scene();
            var camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

            //Rendering the scene to actually see the stuff we code
            var renderer = new THREE.WebGLRenderer();
            renderer.setSize( window.innerWidth, window.innerHeight );
            document.body.appendChild( renderer.domElement );

            //Very simple code for a CUBE
            var geometry = new THREE.BoxGeometry( 1, 1, 1 );
            var material = new THREE.MeshBasicMaterial( { color: 0x00ff00 } );
            var cube = new THREE.Mesh( geometry, material );
            scene.add( cube );


            var animate = function () {
            	requestAnimationFrame( animate );

            	cube.rotation.x += 0.01;
            	cube.rotation.y += 0.01;

            	renderer.render( scene, camera );
            };

            animate();
		</script>
	</body>
</html>
```    
And this is the result.
![Starter Code](https://i.gyazo.com/f0c67cfc5ccc20588d866037e80dc7c1.png)   
My next step toward this is to use what I learn in the videos above to use what I make in Blender and implement it into Three.js. So far, Three.js has not been completely unfamiliar becasue I have already learned the basics of Javascript and a lot about P5.js which is another javascript framework to make games in. However three.js has different syntax that I would need to make myself familiar with, but with practice and learning, I should be able to understand what I code.   

### Skills this project has taught me so far.
Not only am I learning collaboration skills, but I am also developing a stronger growth mindset. Working with somebody has taught me that the beginning will most likely not be a smooth sail, but a rocky start because there needs to be communication between the partners to have a goal that both of you are happy to work on. My partner and I have had a rocky start deciding on what to ultimately use for our project, and we persisted and decided on something that we both wanted to learn more about. This project has already helped in further developing my growth mindset because I realize that I need to have the patience and determination to learn, and learning a new framework and program may be overwhelming, but it is possible. Also, my partner is very knowledgable in javascript, so I learned to not be afriad to ask him for any tips and tricks when programming in this language.    

### Conclusion
Overall, I am pleased with the progress that my partner, Alex, and I have made so far into the project. We have decided together on a project to create using Three.js, Blender, and Typescript. I will be trying my best to learn Three.js and Blender, and I am learning something new every week to make sure I Three.js and Blender well enough to move on from a Prototype and work on the real application.    
[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
