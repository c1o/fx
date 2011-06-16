FX
=====

#### A lightweight and standalone JavaScript library for animation and effects ####

* Perform tween on almost all CSS properties
* Supports both scroll and color animations
* Supports transitional easing
* Multi-unit support (px, em, ex, %, etc.)
* Optionally assign a callback to invoke upon animation completion
* Utility methods include isAnimating and stop
* Supports IE6+, FF, Opera, Safari, and Chrome
* No browser detection

#### Usage ####

	var fx = new FX('element', {
		top: {to: 200},
		left: {to: 200},
		width: {from: 100, to: 200},
		height: {from: 100, to: 200}
	}, 1.3, 'easeOut', callback, this);
	
	fx.start();

FX.Node
=====

#### A drop-in plugin that makes it simple to create and queue animations for a single element ####

* Queue animations
* Helpers methods include fadeIn, fadeOut, highlight, move, and scale
* Utility methods include isAnimating and stop

#### Usage ####

	var node = new FX.Node('element');
	node.animate({		 
		duration: 2,
		transition: 'easeIn',
		attributes: {
			top: {to: 200},
			left: {to: 200},
			width: {from: 100, to: 200},
			height: {from: 100, to: 200}
		},
		callback: function(){
			alert('done!');		
		}
	});

### License ###

FX is licensed under the terms of the MIT License, see the included license.txt file.