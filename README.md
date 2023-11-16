# CSS-Ripple-button


.ripple {
  position: relative;
  overflow: hidden;
  transform: translate3d(0, 0, 0);
}

.ripple:before {
  content: '';
  position: absolute;
  border-radius: 50%;
  width: 50%;
  height: 50%;
  background-color: rgba(255, 255, 255, 0.4); /* White color with transparency */
  transform: translate(-50%, -50%);
  transition: all 0.5s ease-out;
  pointer-events: none;
}

.ripple:hover:before {
  width: 300%; /* Increase size of the ripple effect */
  height: 300%;
  top: 50%;
  left: 50%;
  background-color: rgba(255, 165, 0, 0.4); /* Orange color with transparency */
  transform: translate(-50%, -50%);
}
