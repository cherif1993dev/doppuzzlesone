<div class="game-row">
  <a href="https://html5.gamedistribution.com/98484fa85a944a9e9479be72901fda1f/" class="game-box">
    <img src="https://img.gamedistribution.com/98484fa85a944a9e9479be72901fda1f-512x512.jpeg" alt="Game 1">
    <div class="game-info">
      <h2>Draw Missing Part Puzzle</h2>
    </div>
  </a>
  <a href="https://html5.gamedistribution.com/f9b6d02098bc4f738198ecab632dc602/" class="game-box">
    <img src="https://img.gamedistribution.com/f9b6d02098bc4f738198ecab632dc602-512x512.jpeg" alt="Game 2">
    <div class="game-info">
      <h2>Match Missing Pieces Kids Educational Game</h2>
    </div>
  </a>
</div>
<div class="game-row">
  <a href="https://html5.gamedistribution.com/75ede477cf0243b181ac4e0e09e056bd/" class="game-box">
    <img src="https://img.gamedistribution.com/75ede477cf0243b181ac4e0e09e056bd-512x512.jpeg" alt="Game 3">
    <div class="game-info">
      <h2>Draw The Rest</h2>
    </div>
  </a>
  <a href="https://html5.gamedistribution.com/61377c4361a74aa195a27a44fb0a2f8d/" class="game-box">
    <img src="https://img.gamedistribution.com/61377c4361a74aa195a27a44fb0a2f8d-512x512.jpeg" alt="Game 4">
    <div class="game-info">
      <h2>DOP Puzzle Displace One Part</h2>
    </div>
  </a>
</div>

<div class="app-container">
  <div class="app-label">More Apps</div>
  <div class="app-box touch-scroll">
    <div class="app-icons">
    <a href="#">
      <img src="https://img.gamedistribution.com/bbc23c73b9fe49bfbf36b15bfd6b8ebd-512x512.jpeg" alt="App 1"></a>
	  
	<a href="#">
      <img src="https://img.gamedistribution.com/bbc23c73b9fe49bfbf36b15bfd6b8ebd-512x512.jpeg" alt="App 1"></a>
  </div>
</div>
  </div>


<style>
.game-row {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-bottom: 20px;
}

.game-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 170px;
  height: 190px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0,0,0,0.2);
  overflow: hidden;
  margin: 0px 5px;
  text-decoration: none;
}

.game-box:hover {
  transform: scale(1.1);
}

.game-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.game-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
}

.game-info h2 {
  font-size: 13px;
  margin: 0;
  padding: 0;
  text-align: center;
}

.app-container {
  position: relative;
        top: 40px;
}

.app-container {
  position: relative;
        top: 40px;
		
				/*  hide app-container DIV */
		visibility: hidden;
}

.app-label {
position: relative;
    padding: 1px 5px;
    font-weight: bold;
    background-color: #464646;
    background-color: #f5f5f5;
    color: #464646;
    box-shadow: 0 2px 6px 1px #0000001f ;
}
.app-box {
  width: 310px;
  overflow-x: scroll;
  white-space: nowrap;
  -webkit-overflow-scrolling: touch; /* enable smooth scrolling on iOS */
  padding-top:10px;
}

.app-icons {
  display: inline-block;
  white-space: nowrap;

}

.app-icons a {
  display: inline-block;
  margin-right: 10px;
}

.app-icons a:last-child {
  margin-right: 0;
}

.app-icons img {
  width: 50px;
  height: 50px;
  border-radius: 20px;
}


body{
margin: 0 ;
display: flex ;
user-select: none ;
align-items: center ;
justify-content: center ;
background-color: #e5e7e9 ;
}
.img {
width: 100% ;
flex-shrink: 0;
display: block ;
object-fit: cover ;
}

  </script>
<script>
$(document).ready(function() {
  var isDragging = false;
  var touchX;

  $('.touch-scroll').on('pointerdown', function(e) {
    isDragging = true;
    touchX = e.pageX;
  }).on('pointermove', function(e) {
    if (isDragging) {
      var moveX = e.pageX;
      var diffX = touchX - moveX;
      if (diffX > 0) {
        $(this).scrollLeft($(this).scrollLeft() + diffX);
      } else {
        $(this).scrollLeft($(this).scrollLeft() - Math.abs(diffX));
      }
      touchX = moveX;
    }
  }).on('pointerup', function() {
    isDragging = false;
  }).on('pointerleave', function() {
    isDragging = false;
  });
});


  </script>
