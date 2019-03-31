<div className="item button-parrot">
    <button>Click Me!
        <div className="parrot"></div>
        <div className="parrot"></div>
        <div className="parrot"></div>
        <div className="parrot"></div>
        <div className="parrot"></div>
        <div className="parrot"></div>
    </button>
    <div className="name">Encouragement</div>
</div>

// https://codepen.io/oliviale/pen/vPvvyr?editors=1100
.name
	width: 100%
	text-align: center
	padding: 0 0 3rem
	font: 500 14px 'Rubik', sans-serif
	letter-spacing: .5px
	text-transform: uppercase
	text-shadow: 0 1px 1px rgba(0,0,0,0.4)
.button-parrot
  button
    background-color: #2C3E50
    color: #fff
    border: 3px solid #fff
    border-radius: 50px
    padding: 0.8rem 2rem
    font: 24px "Margarine", sans-serif
    outline: none
    cursor: pointer
    position: relative
    transition: 0.2s ease-in-out
    letter-spacing: 2px
  .parrot
    position: absolute
    width: 60px
    text-align: center
    animation: blink 0.8s 1
    color: transparent
    &:before
      content: "Click Me!"
    &:nth-child(1)
      top: -30px
      left: -40px
      font: 12px/1 "Margarine", sans-serif
      transform: rotate(-20deg)
      animation-duration: 0.5s
    &:nth-child(2)
      font: 12px/1 "Margarine", sans-serif
      right: -40px
      top: -20px
      transform: rotate(15deg)
      animation-duration: 0.3s
    &:nth-child(3)
      font: 16px/1 "Margarine", sans-serif
      top: -60px
      left: 15px
      transform: rotate(10deg)
      animation-duration: 1s
    &:nth-child(4)
      font: 18px/1 "Margarine", sans-serif
      top: -70px
      left: 95px
      transform: rotate(2deg)
      animation-duration: 0.7s
    &:nth-child(5)
      font: 14px/1 "Margarine", sans-serif
      top: 80px
      left: 105px
      transform: rotate(-20deg)
      animation-duration: 0.8s
    &:nth-child(6)
      font: 12px/1 "Margarine", sans-serif
      top: 80px
      left: 5px
      transform: rotate(10deg)
      animation-duration: 1.2s
.button-parrot:hover .parrot:before
  content: "Do it!"
  width: 70px

@keyframes blink
  25%,
  75%
    color: transparent
  40%,
  60%
    color: #2C3E50