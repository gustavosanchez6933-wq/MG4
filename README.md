# MG4
## Devlog
1. The FloatAnimation script works by first starting with private void Start () {_timer = _switchSpeed;} with the timer being the amount of the the fish food has going down and the switching to float back up, and vice versa. The _switchspeeds is how fast the fish food switches to go up or down. Then, using private void (Update), Unity is constantly tracking the floating animation every frame using the combination of if and else statements. Using if (_up) {transform.Translate(0, _moveSpeed * Time.deltaTime, 0);}, Unity is checking if the fish food is going up and if it's false then it continues with the else statement of else { transform.Translate(0, -_moveSpeed * Time.deltaTime, 0);}. However, _timer isn't set up as an acutaly time which is why the coder makde _timer = Time.deltatime to read the time. Then using an if statement, the coder made the timer resets once it reaches less than or equal to 0:  if (_timer <= 0.0f) {_timer = _switchSpeed} Lasttly, by using _up = !up, the code can tell when the animation should switch into another direction.
 
## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)
