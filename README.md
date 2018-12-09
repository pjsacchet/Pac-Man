# Pac-Man
Patrick Sacchet
CS486 (Computer Graphics) Final Project

## Brief Overview
### Objectives
In deciding to recreate a game similar to that of Pac-Man, I knew I wanted to get as close as possible to the real deal.
In order to accomplish this I knew I had to break the game down into smaller pieces, and analyze how they would all fit
together in order to truly create the ultimate Pac-Man experience for the user.

### Execution Plan
My initial plan was as follows:

#### Step 1:
		Create simple circle that moves according to input given by keyboard

#### Step 2:
		Build background/wall structures that will not allow the player model to collide

#### Step 3:
		Add pills to the game-board that will disappear when the player model collides with them

#### Step 4:
		Implement “ghost” models that will move at random, killing the player if they collide

#### Step 5:
		Incorporate sound effects that will be triggered at certain queues (player death, game start, player movement)

#### Step 6: (reach)
		Add complexity to game loop, giving player three lives, presenting a game over screen, etc.

Although I felt as though I had set some pretty substantial goals for myself, I am happy to state that all original
plans were executed and incorporated into my game. With updates to come, I plan to refine and optimize my code in order
to better prevent glitches from occurring and allowing my code to run more efficiently in browsers.

## Reflection/Challenges
Although I am quite satisfied with the product I have produced, there were many challenges that I faced in completing this project.

  1. Object Collision: Although a simple concept, THREEjs no longer incorporates simple methods that allow the user to check for object collision when using geometry objects, so this task was left up to me to accomplish.

  2. Sound Effects/Music: While finding sound effects was not difficult, I did find myself having to manually edit audio files so that each input given by user would play the audio for a suitable amount of time before it would play again.

  3. CORS Issues: While attempting to add audio I also ran into issues regarding the browser's ability to play the sound effects coded. In order to get around this, I had to run a local server manually using the Python command python3 -m http.server which would host a http server on port 8000 where I could access my directory from within my browser.

  4. Ghost Implementation: Incorporating the ghosts was quite the challenge, as they have no real set path in the game. Instead, I gave them the ability to move randomly, incrementing the time between movements appropriately, and detecting collisions with each movement.

## Sources
I am happy to report that all 750 lines of code are mine, but I used various resources throughout the process to properly incorporate this code.

  1. https://stackoverflow.com/questions/27284623/three-js-for-loop-for-every-mesh-in-scene
  2. https://github.com/mrdoob/three.js/issues/9067
  3. https://www.w3schools.com/js/js_popup.asp
  4. https://threejs.org/docs/index.html#manual/en/introduction/How-to-run-things-locally
  5. https://downloads.khinsider.com/game-soundtracks/album/pac-man-arcade
  6. https://japhr.blogspot.com/2013/02/adding-sound-to-threejs-games.html
  7. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/sign
  8. https://threejs.org/docs/#api/en/geometries/PlaneGeometry
  9. https://threejs.org/examples/#webgl_geometry_shapes
  10. https://threejs.org/docs/#api/en/extras/core/Shape
  11. https://threejs.org/docs/#api/en/geometries/PlaneBufferGeometry
  12. https://threejs.org/docs/#api/en/materials/MeshBasicMaterial
  13. https://threejs.org/docs/#api/en/extras/ShapeUtils
  14. https://stackoverflow.com/questions/11473755/how-to-detect-collision-in-three-js
  15. http://learningthreejs.com/data/THREEx/THREEx.KeyboardState.js
  16. https://stackoverflow.com/questions/42958252/how-do-i-move-a-three-js-cube-with-keyboard-input
  17. http://www.threejsgames.com/extensions/#threex.pacman
  18. https://discourse.threejs.org/t/collision-detection-in-three-js/3468
  19. https://www.codingame.com/playgrounds/6181/javascript-arrays---tips-tricks-and-examples
  10. https://answers.unity.com/questions/7615/how-do-i-iterate-over-all-scene-objects-from-an-ed.html
