/* Reset margin and padding */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Main application container */
.app {
  height: 700px; /* Full height of the viewport */
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #74ebd5, #acb6e5); /* Gradient background */
}

/* Background section */
.blurb-background {
  text-align: center;
  padding: 50px;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  background: rgba(255, 255, 255, 0.2); /* Slightly transparent background */
}

/* Card container */
.card-container {
  display: flex;
  justify-content: center;
  gap: 20px; /* Space between cards */
  margin-top: 20px;
}

/* Individual cards */
.card {
  background: rgba(255, 255, 255, 0.1); /* Semi-transparent background */
  border-radius: 10px;
  padding: 20px;
  width: 200px;
  opacity: 0; /* Initially hidden */
  transform: translateY(50px); /* Start slightly below the viewport */
  transition: opacity 0.5s ease, transform 0.5s ease; /* Animation */
  transition: transform 0.3s ease, color 0.3s ease, text-shadow 0.3s ease;

}

/* Hover effect */
.card:hover { 
  transform: translate(10px, -10px);


  /* Bring the hovered card above others */

 }
 
 #font:hover{
  opacity: 1;
  color: black;
 transition: all 0.2s ease-in;
 animation-name: letter;
 animation-duration: 2s;
}

@keyframes letter{
  0%{
    position: relative;
    
    top:10px;
left:70px;


     
   }
  25%{
    position: relative;
    top:10px;
     
   }
  60%{
    position: relative;
    top:10px;

    }
  100%{
    position: relative;
    top:10px;
    }
}
