# Codes
This consists of the various codes right from basic I've learnt throughout my life in various languages.
const player = add([

  sprite('player'),
  scale(0.5),
  pos(20,20),
  body()
])

const MOVE_SPEED = 200
const MOVEMENT_SPEED=400
keyDown('right', () => {
player.move(MOVE_SPEED,0) 
})
keyDown('left', () => {
player.move(-MOVE_SPEED,0) 
})
keyDown('space', () => {
player.move(0,-MOVEMENT_SPEED) 
})




addLevel([
  '                         ',
  '                         ',
  '                         ',
  '                         ',
  '              #          ',
  '              #          ',
  '    #     #   #          ',
  '                         ',
  'xxxxxxxxxxxxxxxxxxxxxxxxx',
  

 
],{
width: 40,
 height: 20,
'x': [sprite('ground'),solid()],
'#': [sprite('enemy'),scale(0.5),body(),'dangerous']
})
player.collides('dangerous', () => {
destroy(player)
})
